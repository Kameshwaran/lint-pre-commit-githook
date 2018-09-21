## Setting up Git pre-commit hook to enforce LINT-ing on source code

1. Copy the file `pre-commit` file from `git-hooks` directory to `.git/hooks` inside your project root directory by running the following command
 `cp git-hooks/pre-commit [Project root path]/.git/hooks/`

2. Open the `.git/hooks/pre-commit` file. Update the language in Line number:4.
  Possible languages are: ruby, javascript, typescript

3. Install the linters
    - If you are ruby, run `gem install rubocop` command
    - If you are on javascript, then run `npm install -g eslint` command
    - If you are on typescript, then run `npm install -g tslint` command
    - You can skip the linter installation, if you have them already installed.

4. Make the file executable by the running the below command.
 `chmod +x .git/hooks/pre-commit`

5. Now, switch to project's root directory and make a tiny commit to check this out!
