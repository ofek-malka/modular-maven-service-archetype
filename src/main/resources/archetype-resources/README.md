# ${artifactId}
${projectDescription}

---

<h2>🏗️ Project Structure</h2>

This is the **starting modular skeleton** for any Maven project generated from this archetype.  
It gives you a clean separation of concerns and a solid foundation to build on.  
You can add more folders, modules, or resources as your project grows.

```
    pom.xml
    README.md
    │
    ├───maven
    │   │   expand-pom.xml
    │   │
    │   ├───build
    │   │       plugins-compile.xml
    │   │       plugins-container.xml
    │   │       plugins-custom.xml
    │   │       plugins-quality.xml
    │   │       plugins-test.xml
    │   │
    │   ├───config
    │   │       app.xml
    │   │       build.xml
    │   │       compiler.xml
    │   │       versions.xml
    │   │
    │   ├───dependencies
    │   │       logging.xml
    │   │       runtime.xml
    │   │       test.xml
    │   │
    │   └───meta
    │           developers.xml
    │           license.xml
    │           project.xml
    │           scm.xml
    │
    └───src
        ├───main
        │   ├───java
        │   │   └───${package.replace('.', '/')}/${mainClass}.java
        │   │           
        │   │
        │   └───resources
        │           log4j2.xml
        │
        └───test
            ├───java
            │   └─── ${package.replace('.', '/')}/Test${mainClass}.java
            │           
            │
            └───resources
                    test-data.txt
```

---


> ⚠️ **Note:** The `maven/` folder is purely a **visual and organizational aid**.  
> It’s not required by Maven itself and can be deleted or reorganized.  
> Its purpose is to **help you maintain a clear mindset** when your project grows bigger or becomes more complex.

---

<h2>🛠️ Modular Maven Setup (Optional)</h2>

The `maven/` directory organizes configuration, dependencies, and build logic separately, giving you a **modular starting point**:

* **`maven/build/`** – Build plugins (compile, test, quality)  
* **`maven/config/`** – Shared project configuration (Java version, build options)  
* **`maven/dependencies/`** – Runtime, test, and logging dependencies  
* **`maven/meta/`** – Project metadata (developers, license, SCM)

> ⚠️ This setup is **optional**. You can remove or reorganize it, but keeping it helps maintain clarity as the project grows.


