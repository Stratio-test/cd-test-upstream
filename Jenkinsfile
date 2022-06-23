@Library('libpipelines@preproduction') _

hose {
    EMAIL = 'cd'
    BUILDTOOLVERSION = '3.5.0'
    VERSIONING_TYPE = 'stratioVersion-3-3'
    UPSTREAM_VERSION = '2.2.0'

    DEV = { config ->
        echo 'THIS IS MASTER'
        doCompile(config)
        doUT(config)
        doPackage(config)
        doStaticAnalysis(config)
        doDeploy(config)
    }     
}
