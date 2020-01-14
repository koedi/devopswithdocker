## When to use Docker and what are the benefits
Docker is an easy way to distribute, try and use different server environments without spending too much time on configuration,
dependencies and polluting your own enviroment. For these purposes Docker offers simple and portable approach. 
Once image is created it will offer same functionality on all platforms. This property makes it an excellent tool for development
as the development environment will the same on all platforms.

Docker container encapsulates the application in a... container. Container contains all necessary dependencies fo the application 
to run as self contained entity. This allows running applications in isolation from the operating system Docker is running on and 
from other containers. 

With Docker development environment can be modified to mimic deployment environment, which will lessen issues with configurations.
Docker and images can be used as version control in development. Tagging with appropriate naming enables version control.
Images can also be used as a part of CI/CD pipeline, where latest development creations are tested, build and deployed automatically.
If service consists of several building blocks any of those can be controlled, developed and maintained separately.

To me Docker (beginner developer in the making) creates several benefits in development pipeline. Production envinronment mimicking,
CI/CD pipeline, portability, isolation and self containment a flexible tool for efficient work.


