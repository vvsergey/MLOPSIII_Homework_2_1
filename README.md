# III. Автоматизация администрирования MLOps II Домашнее задание №2 
# Часть 1: Управление данными с DVC

Результаты выполнения 
```
PS C:\Users\vvser\Documents\УРФУ_СКИЛФЭКТОРИ\MLOPS\III_Automation_MLOps_Administration\Homework_2> dvc repro
Stage 'download' didn't change, skipping
Stage 'process' didn't change, skipping
Running stage 'upload_dataset':
> dvc push
Collecting                                                                                                                                                                                                                                                         |2.00 [00:00,  663entry/s]
Pushing
Everything is up to date.                                                                                                                                                                                                                                                                     
Updating lock file 'dvc.lock'

Running stage 'upload_scripts':
> dvc push
Collecting                                                                                                                                                                                                                                                         |0.00 [00:00,    ?entry/s]
Pushing
Everything is up to date.                                                                                                                                                                                                                                                                     
Updating lock file 'dvc.lock'

dvc dag
WARNING: Unable to find `less` in the PATH. Check out <https://man.dvc.org/pipeline/show> for more info.
   +----------+
   | download |
   +----------+
         *
         *
         *
    +---------+
    | process |
    +---------+
         *
         *
         *
+----------------+
| upload_dataset |
+----------------+
+----------------+
| upload_scripts |
+----------------+
```
