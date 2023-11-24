# Run Jenkins as Docker 
$ docker run --restart always --name jenkins-docker -p 8080:8080 jenkins/jenkins:lts
```
Unable to find image 'jenkins/jenkins:lts' locally
lts: Pulling from jenkins/jenkins
8457fd5474e7: Pull complete 
9e455a0bf7ce: Pull complete 
7746209bfa3a: Pull complete 
b995e8cc8744: Pull complete 
4e039a0e77f3: Pull complete 
b4bc9c3852a0: Pull complete 
30e31170e293: Pull complete 
75ea514c41f0: Pull complete 
64ceedf22f75: Pull complete 
6cd69a5d394b: Pull complete 
67a0cc6a946b: Pull complete 
ca6cd590ac88: Pull complete 
Digest: sha256:c2323612c5da6a2d37f2cd6147b004a4ccceca223a85c07c70bb7ae1f663666a
Status: Downloaded newer image for jenkins/jenkins:lts
Running from: /usr/share/jenkins/jenkins.war
webroot: /var/jenkins_home/war
2023-11-24 17:27:55.728+0000 [id=1]     INFO    winstone.Logger#logInternal: Beginning extraction from war file
2023-11-24 17:27:58.552+0000 [id=1]     WARNING o.e.j.s.handler.ContextHandler#setContextPath: Empty contextPath
2023-11-24 17:27:58.777+0000 [id=1]     INFO    org.eclipse.jetty.server.Server#doStart: jetty-10.0.17; built: 2023-10-02T04:04:10.314Z; git: a0f5f05abaa6c3aabb7c3d35f10a6f412ab8b05f; jvm 17.0.9+9
2023-11-24 17:27:59.281+0000 [id=1]     INFO    o.e.j.w.StandardDescriptorProcessor#visitServlet: NO JSP Support for /, did not find org.eclipse.jetty.jsp.JettyJspServlet
2023-11-24 17:27:59.421+0000 [id=1]     INFO    o.e.j.s.s.DefaultSessionIdManager#doStart: Session workerName=node0
2023-11-24 17:28:00.828+0000 [id=1]     INFO    hudson.WebAppMain#contextInitialized: Jenkins home directory: /var/jenkins_home found at: EnvVars.masterEnvVars.get("JENKINS_HOME")
2023-11-24 17:28:01.071+0000 [id=1]     INFO    o.e.j.s.handler.ContextHandler#doStart: Started w.@27b45ea{Jenkins v2.426.1,/,file:///var/jenkins_home/war/,AVAILABLE}{/var/jenkins_home/war}
2023-11-24 17:28:01.094+0000 [id=1]     INFO    o.e.j.server.AbstractConnector#doStart: Started ServerConnector@37ddb69a{HTTP/1.1, (http/1.1)}{0.0.0.0:8080}
2023-11-24 17:28:01.114+0000 [id=1]     INFO    org.eclipse.jetty.server.Server#doStart: Started Server@43aaf813{STARTING}[10.0.17,sto=0] @6313ms
2023-11-24 17:28:01.120+0000 [id=26]    INFO    winstone.Logger#logInternal: Winstone Servlet Engine running: controlPort=disabled
2023-11-24 17:28:01.763+0000 [id=34]    INFO    jenkins.InitReactorRunner$1#onAttained: Started initialization
2023-11-24 17:28:01.800+0000 [id=36]    INFO    jenkins.InitReactorRunner$1#onAttained: Listed all plugins
2023-11-24 17:28:03.611+0000 [id=32]    INFO    jenkins.InitReactorRunner$1#onAttained: Prepared all plugins
2023-11-24 17:28:03.621+0000 [id=37]    INFO    jenkins.InitReactorRunner$1#onAttained: Started all plugins
2023-11-24 17:28:03.635+0000 [id=33]    INFO    jenkins.InitReactorRunner$1#onAttained: Augmented all extensions
2023-11-24 17:28:04.136+0000 [id=32]    INFO    jenkins.InitReactorRunner$1#onAttained: System config loaded
2023-11-24 17:28:04.137+0000 [id=36]    INFO    jenkins.InitReactorRunner$1#onAttained: System config adapted
2023-11-24 17:28:04.137+0000 [id=36]    INFO    jenkins.InitReactorRunner$1#onAttained: Loaded all jobs
2023-11-24 17:28:04.139+0000 [id=42]    INFO    jenkins.InitReactorRunner$1#onAttained: Configuration for all jobs updated
2023-11-24 17:28:04.227+0000 [id=56]    INFO    hudson.util.Retrier#start: Attempt #1 to do the action check updates server
2023-11-24 17:28:05.314+0000 [id=42]    INFO    jenkins.install.SetupWizard#init: 

*************************************************************
*************************************************************
*************************************************************

Jenkins initial setup is required. An admin user has been created and a password generated.
Please use the following password to proceed to installation:

5177563fd5b74a4385ade195d2e6a381

This may also be found at: /var/jenkins_home/secrets/initialAdminPassword

*************************************************************
*************************************************************
*************************************************************

^C2023-11-24 18:11:42.420+0000 [id=27]  INFO    winstone.Logger#logInternal: JVM is terminating. Shutting down Jetty
2023-11-24 18:11:42.421+0000 [id=27]    INFO    org.eclipse.jetty.server.Server#doStop: Stopped Server@43aaf813{STOPPING}[10.0.17,sto=0]
2023-11-24 18:11:42.426+0000 [id=27]    INFO    o.e.j.server.AbstractConnector#doStop: Stopped ServerConnector@37ddb69a{HTTP/1.1, (http/1.1)}{0.0.0.0:8080}
2023-11-24 18:11:42.428+0000 [id=27]    INFO    hudson.lifecycle.Lifecycle#onStatusUpdate: Stopping Jenkins
2023-11-24 18:11:42.435+0000 [id=27]    INFO    jenkins.model.Jenkins$16#onAttained: Started termination
2023-11-24 18:11:42.454+0000 [id=27]    INFO    jenkins.model.Jenkins$16#onAttained: Completed termination
2023-11-24 18:11:42.455+0000 [id=27]    INFO    jenkins.model.Jenkins#_cleanUpDisconnectComputers: Starting node disconnection
2023-11-24 18:11:42.485+0000 [id=27]    INFO    jenkins.model.Jenkins#_cleanUpShutdownPluginManager: Stopping plugin manager
2023-11-24 18:11:42.485+0000 [id=27]    INFO    jenkins.model.Jenkins#_cleanUpPersistQueue: Persisting build queue
2023-11-24 18:11:42.489+0000 [id=27]    INFO    jenkins.model.Jenkins#_cleanUpAwaitDisconnects: Waiting for node disconnection completion
2023-11-24 18:11:42.489+0000 [id=27]    INFO    hudson.lifecycle.Lifecycle#onStatusUpdate: Jenkins stopped
2023-11-24 18:11:42.490+0000 [id=27]    INFO    hudson.WebAppMain#contextDestroyed: Shutting down a Jenkins instance that was still starting up
java.lang.Throwable: reason
        at hudson.WebAppMain.contextDestroyed(WebAppMain.java:383)
        at org.eclipse.jetty.server.handler.ContextHandler.callContextDestroyed(ContextHandler.java:1059)
        at org.eclipse.jetty.servlet.ServletContextHandler.callContextDestroyed(ServletContextHandler.java:636)
        at org.eclipse.jetty.server.handler.ContextHandler.contextDestroyed(ContextHandler.java:1016)
        at org.eclipse.jetty.servlet.ServletHandler.doStop(ServletHandler.java:306)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.stop(AbstractLifeCycle.java:132)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.stop(ContainerLifeCycle.java:182)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStop(ContainerLifeCycle.java:205)
        at org.eclipse.jetty.server.handler.AbstractHandler.doStop(AbstractHandler.java:97)
        at org.eclipse.jetty.security.SecurityHandler.doStop(SecurityHandler.java:412)
        at org.eclipse.jetty.security.ConstraintSecurityHandler.doStop(ConstraintSecurityHandler.java:413)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.stop(AbstractLifeCycle.java:132)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.stop(ContainerLifeCycle.java:182)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStop(ContainerLifeCycle.java:205)
        at org.eclipse.jetty.server.handler.AbstractHandler.doStop(AbstractHandler.java:97)
        at org.eclipse.jetty.server.session.SessionHandler.doStop(SessionHandler.java:497)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.stop(AbstractLifeCycle.java:132)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.stop(ContainerLifeCycle.java:182)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStop(ContainerLifeCycle.java:205)
        at org.eclipse.jetty.server.handler.AbstractHandler.doStop(AbstractHandler.java:97)
        at org.eclipse.jetty.server.handler.ContextHandler.stopContext(ContextHandler.java:1039)
        at org.eclipse.jetty.servlet.ServletContextHandler.stopContext(ServletContextHandler.java:399)
        at org.eclipse.jetty.webapp.WebAppContext.stopContext(WebAppContext.java:1311)
        at org.eclipse.jetty.server.handler.ContextHandler.doStop(ContextHandler.java:1087)
        at org.eclipse.jetty.servlet.ServletContextHandler.doStop(ServletContextHandler.java:312)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.stop(AbstractLifeCycle.java:132)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.stop(ContainerLifeCycle.java:182)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStop(ContainerLifeCycle.java:205)
        at org.eclipse.jetty.server.handler.AbstractHandler.doStop(AbstractHandler.java:97)
        at org.eclipse.jetty.server.Server.doStop(Server.java:517)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.stop(AbstractLifeCycle.java:132)
        at winstone.Launcher.shutdown(Launcher.java:442)
        at winstone.ShutdownHook.run(ShutdownHook.java:28)
2023-11-24 18:11:42.491+0000 [id=25]    SEVERE  hudson.util.BootFailure#publish: Failed to initialize Jenkins
java.lang.InterruptedException
        at java.base/java.lang.Object.wait(Native Method)
        at java.base/java.lang.Object.wait(Object.java:338)
        at org.jvnet.hudson.reactor.Reactor.execute(Reactor.java:288)
        at jenkins.InitReactorRunner.run(InitReactorRunner.java:49)
        at jenkins.model.Jenkins.executeReactor(Jenkins.java:1205)
        at jenkins.model.Jenkins.<init>(Jenkins.java:992)
        at hudson.model.Hudson.<init>(Hudson.java:86)
        at hudson.model.Hudson.<init>(Hudson.java:82)
        at hudson.WebAppMain$3.run(WebAppMain.java:247)
Caused: hudson.util.HudsonFailedToLoad
        at hudson.WebAppMain$3.run(WebAppMain.java:264)
2023-11-24 18:11:42.499+0000 [id=27]    INFO    o.e.j.s.handler.ContextHandler#doStop: Stopped w.@27b45ea{Jenkins v2.426.1,/,null,STOPPED}{/var/jenkins_home/war}
```