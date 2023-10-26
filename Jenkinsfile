@Library('libpipelines@new-jira-step') _

hose {
    EMAIL = 'cd'
//    FREESTYLE_BRANCHING = true
//     VERSIONING_TYPE = "stratioVersion-3-3"
//     UPSTREAM_VERSION = '0.42.25'

    DEV = { config ->
        doCompile(config)
	doJiraTransition(conf: config, jiraProject: 'TEST1', jiraTransition: 'Done')
        // doUT(config)
        // doPackage(config)
        // doStaticAnalysis(config)
        // doDeploy(config)
	//doDocker(config)
    }     
}
