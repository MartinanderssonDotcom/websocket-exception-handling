WebSocket Exception Handling
---

Demonstrates that GlassFish/Tyrus successfully handles application exceptions occuring in a @ServerEndpoint. WildFly/Undertow force-close the endpoint without even calling @OnClose.

How-to setup this project
---

Just open the project like any other Maven-based Java project. The project uses Arquillian as test runner. The `POM` file include two profiles for GlassFish- and WildFly remote. Thus make sure that either GlassFish or WildFly is running, and have the corresponding maven build profile activated, then just build/test the project and the test application will be deployed and executed live on the server.
