<h2>🏗️ Archetype Structure</h2>
<p>This archetype provides a modular Maven project template.  
The folder structure inside the archetype is organized to separate configuration, metadata, and dependencies for clarity:</p>

<h2>🧩 Generate a Project from This Archetype</h2>
<p>After installing this archetype locally or from a repository, generate a new project using:</p>

<pre><code>mvn archetype:generate \
  -DarchetypeCatalog=true \
  -DaskForDefaultPropertyValues=true \
  -DinteractiveMode=true
</code></pre>

<hr>

<h2>⚙️ Archetype Default Properties</h2>

<p>When generating a new project from this archetype, the following <b>custom properties</b> will be applied automatically if not overridden:</p>

<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Default Value</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>groupId</td><td>com.example</td></tr>
    <tr><td>artifactId</td><td>my-service</td></tr>
    <tr><td>projectDescription</td><td>A modular reactive microservice built with Vert.x and Maven.</td></tr>
    <tr><td>package</td><td>com.example.app</td></tr>
    <tr><td>mainClass</td><td>MainApp</td></tr>
    <tr><td>developerId</td><td>developerId</td></tr>
    <tr><td>developerName</td><td>developerName</td></tr>
    <tr><td>developerEmail</td><td>developerEmail</td></tr>
  </tbody>
</table>

<p><b>🧭 Note:</b><br>
These are the <b>default conventions</b> your archetype enforces.  
Users can override them during generation by passing properties such as:<br>
<code>-DdeveloperName="John Doe"</code> or <code>-DdeveloperEmail="john@example.com"</code>
</p>

<hr>

<h2>📝 Setup</h2>

<p>After generating the project, create a <code>.gitignore</code> file:</p>

<pre><code>cat > .gitignore << 'EOF'
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
</code></pre>

<h2>📄 License</h2>

<p>This project is released under the terms specified in the LICENSE file.</p>
