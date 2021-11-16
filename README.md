# HelloWorld

This is a sample Greengrass v2 component that you can build off on.

Look through the following links first (since they contain important information):
- [Create a Greengrass component](https://docs.aws.amazon.com/greengrass/v2/developerguide/create-components.html)
- [Cat feeder tutorial](https://devopstar.com/2020/12/16/feeding-my-cat-with-aws-iot-greengrassv2)

File structure:
```
.
├── .github
│   └── workflows
│       └── build.yml           : Github Actions build file 
├── README.md
├── com.swarm.HelloWorld.yaml   : Component configuration file
└── src                         : Your source code
    └── main.py                 : The default entry point for your code
```

If you change the name of `main.py`, make sure to update the bottom of your configuration file: `com.swarm.HelloWorld.yaml`.

There's currently a Github workflow set up to automatically deploy this code to S3, although in your own repositories, you can copy files manually.

**NOTE:** There's a specific file structure for artifacts (your code, libraries, etc) described in the AWS docs. That's not reflected in the source code for this repository because the configured Github action does it. Make sure to reconfigure the Github action in your own repository.
