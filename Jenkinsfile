@Library('libpipelines') _

hose {
    EMAIL = 'cd'
    FREESTYLE_BRANCHING = true
    VERSIONING_TYPE = "stratioVersion-2-3"

    DEV = { config ->
        doCompile(config)
        doUT(config)
        doPackage(config)
        doStaticAnalysis(config)
        doDeploy(config)
	doDocker(config)
    }     
}
