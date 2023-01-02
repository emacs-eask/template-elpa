This project was bootstrapped with [eask/cli](https://github.com/emacs-eask/cli).

## How to use?

1. Add any recipes to “recipes” directory like:

  ```elisp
  (package-name :fecher github :repo "username/yourpackage.el")
  ```

2. Prepare to build, this step will install all dependenices before building ELPA:

  ```sh
  eask install
  ```

3. Build archives:

  ```sh
  eask run build
  ```

Regularly, you would want to use:

  ```sh
  eask run update
  ```

This will commit your archives to git repository!

## Available Scripts

In the project directory, you can run:

### `eask run build`

Update ELPA archives without committing them.

### `eask run commit`

Commit ELPA archives.

### `eask run update`

Update ELPA repository.

This is the combination of `build` and `commit` subcommands.

## Learn More

You can learn more in the [github-elpa documentation](https://github.com/10sr/github-elpa).

To learn Eask, check out the [Eask documentation](https://github.com/emacs-eask).
