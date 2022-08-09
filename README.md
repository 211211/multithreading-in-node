## 🧐 How To Use Multithreading in Node.js?

A quick look at the top-level files and directories you'll see in a this project.

    .
    ├── node_modules
    ├── four_workers.js
    ├── index_four_workers.js
    ├── index.js
    ├── worker.js
    ├── package-lock.json
    ├── package.json
    └── README.md

1.  **`/node_modules`**: This directory contains all of the modules of code that your project depends on (npm packages) are automatically installed.

2.  **`index.js`**: Utilizing one worker thread for the CPU-intensive task.

3.  **`worker.js`**: Offloading a CPU-Bound Task with the worker-threads Module.

4.  **`index_four_workers.js`**: Optimizing a CPU-Intensive task using Four worker threads.

5.  **`four_workers.js`**: Optimizing a CPU-Intensive Task Using Four Worker Threads

6. **`package-lock.json`** (See `package.json` below, first). This is an automatically generated file based on the exact versions of your npm dependencies that were installed for your project. **(You won’t change this file directly).**

7. **`package.json`**: A manifest file for Node.js projects, which includes things like metadata (the project’s name, author, etc). This manifest is how npm knows which packages to install for your project.

8. **`README.md`**: A text file containing useful reference information about your project.

# Introduction

You’ll create a Node.js app with a CPU-intensive task that - blocks the main thread. 

Next, you will use the worker-threads module to offload the CPU-intensive task to another thread to avoid blocking the main thread.

Finally, you will divide the CPU-bound task and have four threads work on it in parallel to speed up the task.

# Setting up development environment

1. Install node js for your system (12.X recommended or above)
2. Clone the project

```bash
$ git clone git@github.com:211211/multithreading-in-node.git
$ cd multithreading-in-node

# To run with singly worker thread
$ node index.js

# To run with 4 worker threads
$ node index_four_workers.js

# To measure the calculation time, run the following command
# On Linux
$ time curl --get http://localhost:3000/blocking

# On MacOS, please install gtime via homebrew
$ gtime curl --get http://localhost:3000/blocking
```

## Version 1.0.0

- Initial release

# License

> This project is licensed as open source project.
