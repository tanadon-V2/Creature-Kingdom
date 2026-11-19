# Creature Battle Project (OOP + Git Branching Practice)

This project is designed to help me learn **object-oriented programming** in Python — especially **inheritance** — while also practicing key **Git concepts** like branching, merging, conflict resolution, and version history.

I will begin with a base class (`Creature`) and create additional subclasses on separate Git branches to simulate a real development workflow.

---

## Learning Objectives

### Python / OOP

- Understand and implement **classes**
- Use **inheritance** to extend behaviors
- Override and extend methods (e.g., `attack()`)
- Practice writing simple test code in `main`

### Git / Version Control

- Create and switch branches
- Merge branches into `main`
- Resolve merge conflicts
- View commit history (`git log --graph --all`)

---

## Project Structure

```text
oop_creature_code/
│
├── creature_simulation.py    # Base class + subclasses
└── README.md                 # Project documentation
```

## How to Test and Run

### Requirements

- Python 3
- Git

No external Python libraries are required.

### Running the Program

1. Open the terminal in the `oop_creature_code` directory.
2. Run the following command:

```bash
python creature_simulation.py
```

3. Check the output of the creature tests.

### Classes

**Creature**

The base class containing common attributes and methods.

- `name`: Creature's name
- `hp`: Health points
- `attack_power`: Attack damage
- `attack(target)`: Attacks another creature
- `is_alive()`: Checks whether the creature is alive

**FlyingCreature**

A subclass that can fly and perform aerial attacks.

- `altitude`: Current flying altitude
- `fly_to(new_altitude)`: Changes altitude
- `attack(target)`: Performs an aerial attack

**SwimmingCreature**

A subclass that can dive and perform underwater attacks.

- `depth`: Current underwater depth
- `dive_to(new_depth)`: Changes diving depth
- `attack(target)`: Performs an underwater attack

**FireCreature**

A subclass that can emit fire and perform fire-based attacks.

- `fire_level`: Fire intensity between 0 and 100
- `emit_fire(new_fire_level)`: Updates the fire level
- `attack(target)`: Performs an attack incorporating fire damage

### Testing

The program includes tests for:

- Creature initialization
- Basic attacks
- Health point calculations
- Checking whether a creature is alive
- FlyingCreature abilities
- SwimmingCreature abilities
- FireCreature abilities
- Fire attack damage

### Git Branching and Merging

The project uses separate branches to develop different subclasses:

- `flying_creature`
- `swimming_creature`
- `fire_creature`

Each branch is merged into `main` after development.

To view the commit history, run:

```bash
git log --all --graph --oneline
```

### Push to GitHub

After committing the changes, push the main branch to the remote repository:

```bash
git push origin main
```

## Conclusion

This project demonstrates Python object-oriented programming concepts, including inheritance, method overriding, and code reuse.

It also provides practical experience with Git branching, merging, conflict resolution, and version control.