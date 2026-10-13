# Mission Reflection

This laboratory activity helped me understand how scripting can simplify routine system administration. By using Bash, I learned how to combine commands into a reusable process for creating compressed backups of application data.

I also learned that file permissions affect whether a script can run. Setting the appropriate execution permission is an important step before testing the script. Checking the backup directory afterward helps confirm whether an archive was actually generated.

Another important lesson was the role of Cron in scheduling recurring tasks. A correct schedule and script path are necessary for automated execution. However, adding a Cron entry alone does not prove that the backup will succeed, so the output and resulting files must still be checked.

In an actual system, I would also consider maintaining logs, managing older backup files, and testing whether archived data can be restored. These practices would help improve the reliability of the backup process.

Overall, this activity introduced me to practical automation techniques and showed how Bash and Cron can make repetitive maintenance tasks more consistent and manageable.
