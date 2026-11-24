# Lab Activity 0B: Discussion

## Experience creating and running my first Flutter app

This was my first time creating and running a Flutter app on my own. I created the project with `flutter create cain_mobprog`, opened `lib/main.dart` to look at the starting code, then ran the app with `flutter run`. It was confusing at first because of the folder setup, but it felt good once the app finally launched.

## Challenges with dependencies, SDK configuration, and device selection

Flutter and the SDK were already installed, so I didn't have big problems with dependencies. My main challenge was knowing which folder to run the commands in, since the container folder (`Cain_mobprogAY2627`) is different from the actual project folder. I also had to pay attention to which device to run the app on, since Flutter asks you to choose when there are multiple available.

## Errors encountered and troubleshooting steps

- **`No pubspec.yaml file found`**: I ran `flutter run` in the container folder, not in the project root. I fixed it by creating the project with `flutter create cain_mobprog` and running `cd cain_mobprog` before `flutter run`.
- **`Cannot find path ... cain_mobprog`**: The project folder didn't exist yet, so I had to create it first.
- **`not a git repository`**: I hadn't initialized Git yet. I ran `git init`, then `git add .` and `git commit`.
- **`src refspec main does not match any`**: I had a typo in the remote name (`origiin`) and no commit yet. I removed the wrong remote, made the first commit, then pushed.
- **`Repository not found`**: The remote URL didn't match my real GitHub repository. I copied the correct HTTPS link from the repo page and updated it with `git remote set-url origin`.

## What I learned about executing Flutter applications

- `flutter run` only works inside the project root where `pubspec.yaml` is.
- `flutter doctor` checks if the SDK, editor, and devices are set up properly.
- A device or emulator must be available before the app can run.
- The app starts from `lib/main.dart`.
- Git needs an initial commit and a correct remote URL before pushing.

## Best practices I can apply in the future

- Check my current folder (`dir`) before running commands.
- Run `flutter doctor` first when something seems wrong with the setup.
- Read error messages carefully because they usually tell what the problem is.
- Copy repository URLs directly from GitHub to avoid typos.
- Commit and push after every activity so my work is saved.

## Verification

I verified that the app works by running `flutter run`, checking that the app launched on my selected device without errors in the terminal, and confirming that the app screen displayed properly.