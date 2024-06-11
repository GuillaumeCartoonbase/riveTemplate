# Template Rive Setup

This repository contains the basic setup for a web application integrated with Rive animations.
<br>
The goal of this project is to provide a foundational structure to quickly get started with Rive.

- <a href= "#official-documentation">Official Documentation</a>
- <a href= "#quick-setup">Quick Setup</a>
  - <a href= "#installation">Installation</a>
    - <a href= "#fork-method">Fork Method</a>
    - <a href= "#clone-method">Clone Method</a>
  - <a href= "#usage">Usage</a>
- <a href= "#contributing">Contributing</a>

## Official Documentation

- [Rive Runtime Doc](https://rive.app/community/doc/web-js/docvlgbnS1mp)
- [Rive Support Forum](https://rive.app/community/forums/support/fsnLLkXUaA62)

## Quick Setup

### Installation

#### Fork Method

1. Fork the Template Repository

Fork the template repository to create a copy of it in your own GitHub account for each new project.
<br>
This can be done through the GitHub interface by clicking the "Fork" button on the template repository page.

2. Clone the Forked Repository

Clone the forked repository to your local machine.

```bash
git clone https://github.com/yourusername/project1.git
cd project1
```

3. Set Up the Upstream Remote

Add the original template repository as an upstream remote. This allows you to pull in changes from the template repository later.

```bash
git remote add upstream https://github.com/GuillaumeCartoonbase/riveTemplate.git
```

4. Make Changes and Develop Your Project

Develop your project as needed, committing and pushing changes to your forked repository.

5. Pull Changes from the Template Repository

When there are updates in the template repository, you can pull these updates into your forked repository.

```bash
git fetch upstream
git merge upstream/main
```

6. Resolve Conflicts if Necessary

If there are any conflicts between the changes in your project and the updates from the template, Git will prompt you to resolve them.
<br>
After resolving conflicts, commit the merge.

```bash
git commit -m "Merged updates from template"
```

#### Clone Method

1. Create a New Repository

First, create a new repository on GitHub where you want to duplicate your existing repository.
<br>
Name the new repository with a new name.

2. Clone the Original Repository

Clone the original repository to your local machine:

```bash
git clone https://github.com/GuillaumeCartoonbase/riveTemplate.git
```

3. Rename the Remote

Rename the `origin` remote to `upstream`:

```bash
git remote rename origin upstream
```

4. Add the New Repository as a Remote

Add the new repository as a remote called `origin`:

```bash
git remote add origin https://github.com/yourusername/project1.git
```

5. Push to the New Repository

Push all branches and tags to the new repository:

```bash
git push -u origin --all
git push -u origin --tags
```

##### Keeping the Fork Updated

To keep your forked repository (`project1`) updated with changes from the original repository (`riveTemplate`), you can regularly pull in changes.

1. Fetch and Merge Updates

To pull in updates from the original repository, use the following commands:

```bash
git fetch upstream
git merge upstream/main
```

2. Resolve Conflicts

If there are any conflicts, Git will prompt you to resolve them. After resolving conflicts, commit the merge:

```bash
git commit -m "Merged updates from template"
```

### Usage

- **project .riv**
  - Place your .riv file in the `src/` directory
- **index.html**
  - Edit the `<canvas>` width and height for your project
- **src/rive.js**
  1. Edit the line `src: "src/.riv",` to point to the correct .riv
  2. Edit the line `stateMachines: "State Machine 1",` to setup your state machine name

## Contributing

Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please submit a pull request.
<br>
For major changes, please open an issue first to discuss what you would like to change.
