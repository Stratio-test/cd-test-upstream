@Library('libpipelines') _

hose {
    EMAIL = 'cd'
    FREESTYLE_BRANCHING = true
    UPSTREAM_VERSION = '0.42'
    VERSIONING_TYPE = "stratioVersion-2-3"

    DEV = { config ->
        doCompile(config)
        doUT(config)
        doPackage(config)
        doStaticAnalysis(config)
        doDeploy(config)
	doDocker(conf: config, dockerfile: "Dockerfile.test")
    }     
}
