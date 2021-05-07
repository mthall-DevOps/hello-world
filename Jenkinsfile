properties([
    
    parameters([
        choice(choices: ['Yes', 'No'], description: 'Enter your Answer(Yes/No)', name: 'Answer'), 
        string(defaultValue: 'Mani', description: 'Enter Full Name', name: 'Name', trim: false)
        ])
        ])
        
if(name=='Yes'){
    j_node = 'master'
}
else{
    j_node = 'slave'
}
    
node(j_node){
    stage('Build and Package'){
    echo 'Build and package'
    echo "choice: ${params.Answer}"
    }
    
    stage('QA Test'){
    echo 'Tetsing in QA'
    echo "choice: ${params.Name}"
    }
}
