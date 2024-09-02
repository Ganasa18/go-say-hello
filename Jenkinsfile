@Library('global-jenkins-pipe@master') _
pipeline {
    // Call the global pipeline function
    globalPipeline(
        projectName: 'go-say',
        createHelm: 'true',
        backwardHelm: false,
        projectType: 'laravel',
        shouldRunJavaUnitTest: false,
        shouldRunJavaIntegrationTest: false,
        shouldRunGoUnitTest: false
    )
}
