@Library('libpipelines@preproduction') _

hose {
    EMAIL = 'cd'
    VERSIONING_TYPE = "stratioVersion-3-3-3"
    UPSTREAM_VERSION = '2.2.1_0.1.0'

    DEV = { config ->
        doCompile(config)
        doUT(config)
        doPackage(config)
        doStaticAnalysis(config)
        doDeploy(config)
	doDocker(config)
    }     
}
