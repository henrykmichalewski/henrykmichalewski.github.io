# Installation Instructions for Debian/Ubuntu

To run this Jekyll site locally, you need to install Ruby and the necessary build tools.

## 1. Install System Dependencies

Open your terminal and run:

```bash
sudo apt update
sudo apt install ruby-full build-essential zlib1g-dev
```

*   `ruby-full`: Installs Ruby and necessary development headers.
*   `build-essential`: Required for compiling native extensions (like the `json` gem).
*   `zlib1g-dev`: Required for some Jekyll dependencies.

## 2. Install Jekyll and Bundler

Install the Ruby gems for Jekyll and Bundler. It is recommended to install them for your user to avoid permission issues:

```bash
gem install jekyll bundler --user-install
```

**Important**: You need to ensure the gem executable directory is in your `PATH`.

1.  Add the following line to your shell configuration file (e.g., `~/.bashrc` or `~/.zshrc`):
    ```bash
    export PATH="$HOME/.local/share/gem/ruby/3.2.0/bin:$PATH"
    ```
    *(Note: The version `3.2.0` may vary. Check your version with `ruby -v` or look in `~/.local/share/gem/ruby/`)*

2.  Apply the changes:
    ```bash
    source ~/.bashrc
    ```

## 3. Install Project Dependencies

Navigate to the project directory (`minimal-light`) and run:

```bash
bundle install
```

## 4. Run the Site

Start the local server:

```bash
bundle exec jekyll serve
```

You can then view your website at `http://localhost:4000`.
