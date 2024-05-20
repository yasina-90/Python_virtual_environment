<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Python venv Virtual Environment Cheat Sheet</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2, h3 {
            color: #333;
        }
        pre {
            background-color: #f4f4f4;
            padding: 10px;
            border-radius: 5px;
            overflow-x: auto;
        }
        code {
            font-family: "Courier New", Courier, monospace;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Python venv Virtual Environment Cheat Sheet</h1>

        <h2>What is a Virtual Environment?</h2>
        <p>
            A virtual environment in Python is a self-contained directory that includes a Python installation and a collection of installed packages. It allows you to create isolated environments for different projects, ensuring that each project has its own dependencies and does not interfere with other projects. This is particularly useful when working on multiple projects that require different versions of the same packages.
        </p>

        <h2>1. Create a Virtual Environment</h2>
        <p>
            To create a virtual environment, navigate to the root directory of your project and run the following command:
        </p>
        <pre><code>python -m venv qed-venv</code></pre>
        <p>This command creates a virtual environment named <code>qed-venv</code> in your project directory.</p>

        <h2>2. Activate the Virtual Environment</h2>
        <p>Activating the virtual environment changes your shell's environment so that it uses the Python and pip executables installed inside the virtual environment instead of the global ones.</p>
        <h3>On Windows:</h3>
        <pre><code>.\qed-venv\Scripts\activate</code></pre>
        <h3>On macOS/Linux:</h3>
        <pre><code>source qed-venv/bin/activate</code></pre>
        <p>After activation, your shell prompt will typically change to indicate that the virtual environment is active.</p>

        <!-- Skipping steps 3, 4, 5, 6 for brevity -->

        <h2>7. Delete the Virtual Environment</h2>
        <p>If you no longer need the virtual environment and want to delete it, simply remove the <code>qed-venv</code> directory.</p>
        <h3>On Windows:</h3>
        <p>Open File Explorer, navigate to your project directory, and delete the <code>qed-venv</code> folder.</p>
        <h3>On macOS/Linux:</h3>
        <pre><code>rm -rf qed-venv</code></pre>
        <p>This will completely remove the virtual environment from your project directory.</p>

        <h2>Summary</h2>
        <ul>
            <li>Create a virtual environment: <code>python -m venv qed-venv</code></li>
            <!-- List other steps -->
        </ul>
        <p>By following these steps, you can easily manage your Python project's dependencies, ensure a consistent development environment across different machines, and clean up when the virtual environment is no longer needed.</p>
    </div>
</body>
</html>
