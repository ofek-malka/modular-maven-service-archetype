# ${artifactId}
${projectDescription}

---

<h2>🏗️ Project Structure</h2>

The project is organized in a modular and conventional manner for maintainability and adherence to best practices:
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

<h2>🛠️ Modular Maven Setup</h2>

This project uses a modular Maven setup by offloading configuration details to the `maven/` directory.

* **`maven/build/`**: Build plugins (compilation, testing, quality checks)
* **`maven/config/`**: Shared configuration (Java version, build options)
* **`maven/dependencies/`**: Separated runtime and test dependencies
* **`maven/meta/`**: Project metadata (developers, license, SCM)

---

<h2>🚀 Build and Run</h2>

<h3>Build the project</h3>
```bash
mvn clean install
```


<h2>🧩 Generate a new project (from archetype)</h2>

<h3>Use this command for interactive setup:</h3>
```bash
mvn archetype:generate \
  -DarchetypeCatalog=true \
  -DaskForDefaultPropertyValues=true \
  -DinteractiveMode=true
```

---

<h2>👤 Developer Information</h2>

| Field | Value |
| :--- | :--- |
| **Name** | ${developerName} |
| **Email** | ${developerEmail} |
| **ID** | ${developerId} |

---


<h2> 📝 Setup </h2>

After generating the project, create a `.gitignore` file:

\`\`\`bash
cat > .gitignore << 'EOF'
target/
*.class
*.jar
*.war
*.ear
*.log
.idea/
*.iml
.vscode/
.DS_Store
EOF
\`\`\`


<h2>📄 License</h2>

This project is released under the terms specified in the LICENSE file.
