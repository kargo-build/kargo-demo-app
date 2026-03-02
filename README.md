# 🎉 Kargo Demo Application 🚀

Welcome to the **Kargo Demo Application**! This project is here to show you just how incredibly *easy* and *powerful* it is to build Kotlin/Native applications using [Kargo](https://github.com/kargo-build/kargo)! 

Get ready to say goodbye to complex build setups and hello to seamless development! ✨

## 🌟 Awesome Features

- **Blazing Fast Kotlin/Native:** Compiles straight to a standalone, native Linux executable! 🏎️💨
- **Zero Config Git Dependencies:** Watch the magic happen as Kargo fetches and uses a library *directly* from a Git repository (`github: kargo-build/kargo-native-git-lib`)! No publishing needed! 🤯
- **Unbelievably Simple:** Just one tiny `module.yaml` file to rules it all!

## 🛠️ Prerequisites (It's so simple!)

To experience the magic, you just need:

- **Kargo**: You don't even need to install anything! Just use the `./kargo` wrapper script included right here! 
- A Linux environment (configured for `linuxX64`).

## ⚡ Setup & Build in Seconds

1. **Clone it!**
   ```bash
   git clone <repository-url>
   cd kargo-demo-app
   ```

2. **Build it with ONE command:**
   Watch as Kargo effortlessly resolves dependencies, fetches Git libraries, and compiles everything for you! 🪄

   ```bash
   ./kargo build
   ```

   Boom! 💥 Your compiled standalone executable is ready and waiting at `dist/app.kexe`.

## 🚀 Run It!

You can run your shiny new application like this:

1. **Directly execute the binary:**
   ```bash
   ./dist/app.kexe
   ```

2. **Or let Kargo run it for you:**
   ```bash
   ./kargo run
   ```

You should see this glorious output:
```
Hello, World! (from git source)
```
*Yes, that string came all the way from another Git repository! How cool is that?!* 😎

## 📂 Project Structure (No bloat here!)

- `module.yaml`: The absolute MVP! This tiny configuration file defines what we're building and magically tells Kargo to grab our Git dependency!
- `src/com/example/demo/main.kt`: The main application code that uses a class (`Greeter`) cheerfully fetched from the internet!
- `kargo`: Your handy-dandy wrapper script!

## 🧠 How the Magic Works

Take a look at `module.yaml`! It literally just says it needs the `kargo-build/kargo-native-git-lib` repo. When you run Kargo, it automatically goes out to the web, brings down the repository, compiles it, and links it directly into your `app.kexe`! 

The future of Kotlin/Native builds is here, and it's spectacular! 🎉
