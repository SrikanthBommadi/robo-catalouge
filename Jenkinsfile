// @Library('jenkins-shared-library')_

// def configMap = [
//     project: "roboshop",
//     component: "catalogue"
// ]

// if ( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
//     nodeJSEKSPipeline(configMap)
// }
// else{
//     echo "Please follow production process"
// }

@Library('jenkins-shared-library') _

def configMap = [
    project: "roboshop",
    component: "catalogue"
]

// Use safe null check and make sure BRANCH_NAME is available
if (env.BRANCH_NAME?.toLowerCase() != 'main') {
    nodeJSEKSPipeline(configMap)
} else {
    echo "Please follow production process"
}
