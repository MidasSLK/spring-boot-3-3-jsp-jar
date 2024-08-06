### Spring boot 3.3 serving jsp files and run as a jar file
Recently, I ran into an issue with a colleague trying to upgrade some old jsp-based projects to use spring boot and run them in containers. This repo provides examples of how to get a jsp application using spring-boot and running an embedded tomcat servlet container to be packaged and run as a jar.

It contains maven projects. The application runs with an embedded tomcat container and a jar packaging. 
`
- This is not straight-forward due to certain [limitations][1] with jsps

If for whatever reason, you can't deal with a war packaging, there's a bit of a hack you can try. 
Credit to [this guy][4] here for providing some code and hints for a solution to version 3.3 of spring boot.
Credit to [this guy][3] here for doing this for the version 2 of spring boot.
Credit to [this guy][2] here for doing this for the even older versions of spring boot.

[1]: https://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-developing-web-applications.html#boot-features-jsp-limitations
[2]: http://hengyunabc.github.io/spring-boot-fat-jar-jsp-sample/
[3]: https://github.com/code4kix/spring-boot-examples
[4]: https://stackoverflow.com/a/78619625
