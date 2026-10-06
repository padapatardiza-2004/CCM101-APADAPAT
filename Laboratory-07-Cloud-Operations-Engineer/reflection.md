# Mission Reflection

This laboratory activity helped me understand why checking the host server is important even when the containers are working properly. I learned that containers still depend on the resources of the host server, so problems with memory, CPU, or disk space can also affect the applications running inside them. Before this activity, I mostly focused on whether the application was working or not, but I now understand that checking the server's resources can help identify possible problems before they become serious.

I also learned how useful the `docker logs` command can be when troubleshooting an application. If a user cannot log into a web application, checking the logs can provide information about errors, failed requests, or other events that happened inside the container. This is helpful because instead of guessing what went wrong, I can use the recorded information to investigate the problem.

Another thing I learned is the difference between logs and metrics. Logs show what happened in the application, such as requests and errors, while metrics show numerical information about the container's performance, such as CPU and memory usage. I realized that both are important because they provide different information that can help when checking an application's condition.

For large companies that manage thousands of containers, I think tools such as Prometheus and Grafana would be useful because they can collect and display information from many systems in one place. This would make monitoring a large number of containers easier and more organized.

Overall, this activity improved my confidence in using Linux and Docker commands. I became more familiar with `free`, `df`, `top`, `curl`, `docker logs`, and `docker stats`. I also learned that troubleshooting is easier when I look at actual system information instead of just guessing what the problem might be.
