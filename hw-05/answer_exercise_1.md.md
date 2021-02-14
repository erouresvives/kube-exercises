--------------------------------------------------
1. instalacion / despliegue de jenkins
--------------------------------------------------
docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts

        docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts
        Unable to find image 'jenkins/jenkins:lts' locally
        lts: Pulling from jenkins/jenkins
        0ecb575e629c: Pull complete
        57cd93315d96: Pull complete
        8f2fb5ba5578: Pull complete
        5df25027d832: Pull complete
        2721a364269e: Pull complete
        b81a9d475179: Pull complete
        84f09918e1fd: Pull complete
        39e6b9a64e2c: Pull complete
        978144699edc: Pull complete
        75e164ae7556: Pull complete
        284ba7d0aa91: Pull complete
        dd9e2842d0a9: Pull complete
        42884ffea68b: Pull complete
        1107f24019e2: Pull complete
        32a343a0ab7c: Pull complete
        fcaf2e003df7: Pull complete
        Digest: sha256:641eeb472ab94bc89e7e6f2e6d337f4c38a934d707a9f02713bbb1227b3a08dd
        Status: Downloaded newer image for jenkins/jenkins:lts
        Running from: /usr/share/jenkins/jenkins.war
        webroot: EnvVars.masterEnvVars.get("JENKINS_HOME")
        2021-02-13 19:56:53.690+0000 [id=1]     INFO    org.eclipse.jetty.util.log.Log#initialized: Logging initialized @211ms to org.eclipse.jetty.util.log.JavaUtilLog
        2021-02-13 19:56:53.769+0000 [id=1]     INFO    winstone.Logger#logInternal: Beginning extraction from war file
        2021-02-13 19:56:54.557+0000 [id=1]     WARNING o.e.j.s.handler.ContextHandler#setContextPath: Empty contextPath
        2021-02-13 19:56:54.595+0000 [id=1]     INFO    org.eclipse.jetty.server.Server#doStart: jetty-9.4.33.v20201020; built: 2020-10-20T23:39:24.803Z; git: 1be68755656cef678b79a2ef1c2ebbca99e25420; jvm 1.8.0_282-b08
        2021-02-13 19:56:54.762+0000 [id=1]     INFO    o.e.j.w.StandardDescriptorProcessor#visitServlet: NO JSP Support for /, did not find org.eclipse.jetty.jsp.JettyJspServlet
        2021-02-13 19:56:54.789+0000 [id=1]     INFO    o.e.j.s.s.DefaultSessionIdManager#doStart: DefaultSessionIdManager workerName=node0
        2021-02-13 19:56:54.790+0000 [id=1]     INFO    o.e.j.s.s.DefaultSessionIdManager#doStart: No SessionScavenger set, using defaults
        2021-02-13 19:56:54.791+0000 [id=1]     INFO    o.e.j.server.session.HouseKeeper#startScavenging: node0 Scavenging every 660000ms
        2021-02-13 19:56:55.018+0000 [id=1]     INFO    hudson.WebAppMain#contextInitialized: Jenkins home directory: /var/jenkins_home found at: EnvVars.masterEnvVars.get("JENKINS_HOME")
        2021-02-13 19:56:55.085+0000 [id=1]     INFO    o.e.j.s.handler.ContextHandler#doStart: Started w.@2a492f2a{Jenkins v2.263.4,/,file:///var/jenkins_home/war/,AVAILABLE}{/var/jenkins_home/war}
        2021-02-13 19:56:55.101+0000 [id=1]     INFO    o.e.j.server.AbstractConnector#doStart: Started ServerConnector@5c86a017{HTTP/1.1, (http/1.1)}{0.0.0.0:8080}
        2021-02-13 19:56:55.101+0000 [id=1]     INFO    org.eclipse.jetty.server.Server#doStart: Started @1622ms
        2021-02-13 19:56:55.102+0000 [id=33]    INFO    winstone.Logger#logInternal: Winstone Servlet Engine running: controlPort=disabled
        2021-02-13 19:56:56.032+0000 [id=40]    INFO    jenkins.InitReactorRunner$1#onAttained: Started initialization
        2021-02-13 19:56:56.051+0000 [id=59]    INFO    jenkins.InitReactorRunner$1#onAttained: Listed all plugins
        2021-02-13 19:56:56.893+0000 [id=68]    INFO    jenkins.InitReactorRunner$1#onAttained: Prepared all plugins
        2021-02-13 19:56:56.898+0000 [id=43]    INFO    jenkins.InitReactorRunner$1#onAttained: Started all plugins
        2021-02-13 19:56:56.904+0000 [id=54]    INFO    jenkins.InitReactorRunner$1#onAttained: Augmented all extensions
        2021-02-13 19:56:57.430+0000 [id=54]    INFO    jenkins.InitReactorRunner$1#onAttained: System config loaded
        2021-02-13 19:56:57.430+0000 [id=63]    INFO    jenkins.InitReactorRunner$1#onAttained: System config adapted
        2021-02-13 19:56:57.430+0000 [id=42]    INFO    jenkins.InitReactorRunner$1#onAttained: Loaded all jobs
        2021-02-13 19:56:57.431+0000 [id=52]    INFO    jenkins.InitReactorRunner$1#onAttained: Configuration for all jobs updated
        2021-02-13 19:56:57.436+0000 [id=82]    INFO    hudson.model.AsyncPeriodicWork#lambda$doRun$0: Started Download metadata
        2021-02-13 19:56:57.442+0000 [id=82]    INFO    hudson.util.Retrier#start: Attempt #1 to do the action check updates server
        2021-02-13 19:56:57.908+0000 [id=52]    INFO    o.s.c.s.AbstractApplicationContext#prepareRefresh: Refreshing org.springframework.web.context.support.StaticWebApplicationContext@5244951e: display name [Root WebApplicationContext]; startup date [Sat Feb 13 19:56:57 UTC 2021]; root of context hierarchy
        2021-02-13 19:56:57.908+0000 [id=52]    INFO    o.s.c.s.AbstractApplicationContext#obtainFreshBeanFactory: Bean factory for application context [org.springframework.web.context.support.StaticWebApplicationContext@5244951e]: org.springframework.beans.factory.support.DefaultListableBeanFactory@72fda86c
        2021-02-13 19:56:57.917+0000 [id=52]    INFO    o.s.b.f.s.DefaultListableBeanFactory#preInstantiateSingletons: Pre-instantiating singletons in org.springframework.beans.factory.support.DefaultListableBeanFactory@72fda86c: defining beans [authenticationManager]; root of factory hierarchy
        2021-02-13 19:56:58.085+0000 [id=52]    INFO    o.s.c.s.AbstractApplicationContext#prepareRefresh: Refreshing org.springframework.web.context.support.StaticWebApplicationContext@728a6e56: display name [Root WebApplicationContext]; startup date [Sat Feb 13 19:56:58 UTC 2021]; root of context hierarchy
        2021-02-13 19:56:58.086+0000 [id=52]    INFO    o.s.c.s.AbstractApplicationContext#obtainFreshBeanFactory: Bean factory for application context [org.springframework.web.context.support.StaticWebApplicationContext@728a6e56]: org.springframework.beans.factory.support.DefaultListableBeanFactory@65fc41ab
        2021-02-13 19:56:58.086+0000 [id=52]    INFO    o.s.b.f.s.DefaultListableBeanFactory#preInstantiateSingletons: Pre-instantiating singletons in org.springframework.beans.factory.support.DefaultListableBeanFactory@65fc41ab: defining beans [filter,legacy]; root of factory hierarchy
        2021-02-13 19:56:58.306+0000 [id=52]    INFO    jenkins.install.SetupWizard#init:

        *************************************************************
        *************************************************************
        *************************************************************

        Jenkins initial setup is required. An admin user has been created and a password generated.
        Please use the following password to proceed to installation:

        7de1b138a6b04ced85af91989c5f5626

        This may also be found at: /var/jenkins_home/secrets/initialAdminPassword

        *************************************************************
        *************************************************************
        *************************************************************

        2021-02-13 19:57:03.142+0000 [id=82]    INFO    h.m.DownloadService$Downloadable#load: Obtained the updated data file for hudson.tasks.Maven.MavenInstaller
        2021-02-13 19:57:03.143+0000 [id=82]    INFO    hudson.util.Retrier#start: Performed the action check updates server successfully at the attempt #1
        2021-02-13 19:57:03.145+0000 [id=82]    INFO    hudson.model.AsyncPeriodicWork#lambda$doRun$0: Finished Download metadata. 5,708 ms
        2021-02-13 19:57:03.939+0000 [id=54]    INFO    jenkins.InitReactorRunner$1#onAttained: Completed initialization
        2021-02-13 19:57:03.949+0000 [id=30]    INFO    hudson.WebAppMain$3#run: Jenkins is fully up and running

--------------------------------------------------
2. Configuración
--------------------------------------------------

* Acceder a localhost:8080 (01.png)
    Introducir la contraseña proporcionada en la instalación, en este caso: 
    7de1b138a6b04ced85af91989c5f5626

* Procedemos a la instalación de Jenkins
    Seleccionamos instalar suggested pluggins

* Al finalizar la instalación (02.png), creamos un nuevo usuario administrador (03.png)
* Finalizada la creación, establecemos la configuración de la instancia (04.png) -> todo OK (05.png)

* Instalar los plugins de docker y docker pipeline en:
    - Administrar Jenkins -> Administrar Plugins

--------------------------------------------------
3. Creación Pipeline
--------------------------------------------------

* Añadimos en nuestro repositorio git el fichero Jenkinsfile, junto a la aplicación (06.png)
    - Recuperamos en enlace dentro de Code, lo necesitaremos en Jenkins

En Jenkins

* Seleccionamos crear una nueva tarea, la primera opción del menú (07.png) 
* Seleccionamos como opción "Pipeline", y llamaremos a la tarea "Pipeline_Entregable_CI_CD" (08.png)

* En la zona Pipeline -> Definition, seleccionamos la opción "Pipeline script from SCM".
    * SCM: git
    * en Repository URL indicamos la url del repositorio con el jenkinsfile del punto anterior
        https://github.com/erouresvives/kube-exercises.git 
    * nos aseguramos que Jenkinsfile aparezca en el campo Script Path
    * Guardar (09.png)

-------------------------------------
4. Build
-------------------------------------

* Construir ahora para lanzar la build (10.png)


* En caso de que todo fuera correcto visualizariamos lo siguiente, las imagenes corresponden a un intento solo con los stage (11.png)

--------------------------------------------------
ERROR (12.png)
--------------------------------------------------
- Hasta aquí he conseguido llegar, a pesar de intentar con múltiples ficheros tanto propios como de internet, con echo de los comandos, sin el echo (como esta ahora), instalar todos los plugins disponibles y cualquier otra idea que me viniera a la mente, no he conseguido salir del error

...script.sh: docker: not found

--------------------------------------------------


Started by user admin
Obtained Jenkinsfile from git https://github.com/erouresvives/kube-exercises.git
Running in Durability level: MAX_SURVIVABILITY
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /var/jenkins_home/workspace/Pipeline_Entregable_CI_CD
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --is-inside-work-tree # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/erouresvives/kube-exercises.git # timeout=10
Fetching upstream changes from https://github.com/erouresvives/kube-exercises.git
 > git --version # timeout=10
 > git --version # 'git version 2.20.1'
 > git fetch --tags --force --progress -- https://github.com/erouresvives/kube-exercises.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/master^{commit} # timeout=10
Checking out Revision ba85f3b03f0ba0dfa9f511d9807391e69dbf7d00 (refs/remotes/origin/master)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f ba85f3b03f0ba0dfa9f511d9807391e69dbf7d00 # timeout=10
Commit message: "Update Jenkinsfile"
 > git rev-list --no-walk 8e2d0b4c9d8b5ad54dcc34ed2be1980a32f82f7d # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] isUnix
[Pipeline] sh
+ docker inspect -f . node:alpine
/var/jenkins_home/workspace/Pipeline_Entregable_CI_CD@tmp/durable-9d3120cd/script.sh: 1: /var/jenkins_home/workspace/Pipeline_Entregable_CI_CD@tmp/durable-9d3120cd/script.sh: docker: not found
[Pipeline] isUnix
[Pipeline] sh
+ docker pull node:alpine
/var/jenkins_home/workspace/Pipeline_Entregable_CI_CD@tmp/durable-8824e008/script.sh: 1: /var/jenkins_home/workspace/Pipeline_Entregable_CI_CD@tmp/durable-8824e008/script.sh: docker: not found
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
ERROR: script returned exit code 127
Finished: FAILURE
