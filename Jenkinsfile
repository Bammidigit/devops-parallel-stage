pipleline
{agent any
stages
{
    stage ('execute script parallelly')
    {
        parallel
        {
          stage ('run phython script')
          { steps {sh 'echo python_script_is_running'}}
          stage ('run schell script')
          {steps {sh 'echo shell_script_is_running'}}
        }

    }
    stage ('publish python and shell script logs to shared location')
    {steps {sh 'echo upload_logs_to_shared_location'}}
}
}
