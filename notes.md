# Dev notes

Welcome to my personal dev notes <br />
Started on 25/01/2023, this is a bunch of my most used references, snippets, ideas and links that can be used to go back to whenever they are needed.

## **Javascript**

- Find what class an object is: `[obj].constructor.name`
- For checking if a string is equal to many options you can use `[1, 2, 3, 4, 5, ...].includes(stringToMatch);`

## **Typescript**

## **Node**

## **SQL**

- Database basics: https://support.microsoft.com/en-us/office/database-design-basics-eb2159cf-1e30-401a-8084-bd4f9c9ca1f5
- Show more detailed error messages:
  ```sql
  SHOW ENGINE INNODB STATUS
  ```

## **Git**

- `git log --oneline -n [x]` shows x most recent commits (oneline makes it easier to read, and see more info)
- `git restore [--staged]` to restore unstaged/staged changes (depending on the flag)
- `git stash` -> `git checkout [branch]` -> `git stash pop` to move uncommited changes to a different branch
- `git add -p` / `git commit -p` to add/commit files more accurately without accidentally leaving in stupid stuff. Can just use `git commit -p` to skip over the adding stage
- General workflow:
  ```
  git status (check what's tracked/untracked and what's in the staging area)
  git pull --rebase
  git add -p / git add [files]
  git commit -m "prefix: description (#ticket)"
  git push
  ```

## **Linux**

- `lsof -i [portNumber]` to check processes on port

## **VSCode**

- Essential / recommended extensions:

  - `[Theme]`: Atom One Dark
  - `[HTML]`: Auto Rename Tag
  - `[HTML]`: Live server
  - `[HTML]`: Emmet
  - `[CSS]`: Color Highlight
  - `[Formatting]`: ESLint
  - `[Formatting]`: StyleLint
  - `[Formatting]`: Prettier
  - `[Formatting]`: TODO Highlight V2
  - `[Formatting]`: Code Spell Checker
  - `[General]`: TabOut
  - `[General]`: PX to REM
  - `[General]`: Import const
  - `[Language]`: Babel Javascript
  - `[Language]`: IntelliCode
  - `[Language]`: Svelte 3 snippets
  - `[Language]`: Svelte for VS Code
  - `[Language]`: Pylance
  - `[Language]`: Python

- `ctrl+g` to go to a specific line in the file

## **Docker**

There are 3 main basic parts to docker

- dockerfile, image & container
  - dockerfile is the instructions on how to build an image
  - image is the "executable" which builds into a container
  - container is the physical running process of your image
