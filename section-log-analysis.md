SSH logs:
    The hostname of the ssh server is located right after the timestamp.
    

nginx access log:
    cat <file_name> | cut -d " " -f 1 | sort | uniq -c | wc -l                          //Should find all unique IPs in a log file
    cat <file_name> | cut -d '"' -f3 | cut -d ' ' -f2 | sort | uniq -c | sort -rn       //Should find all requests in a log file
    awk -F" " '{print $6}' <file_name> | sort | uniq -c                                 //Should prints all HTTP methods in a log file and shows amount of each one

    Note: This commands may need to edited for different lines/values.
    This is just what I found that worked.

squid proxy log:
    cat squid_access.log | awk '{print $2}' | sort -n           //Should sort through access times
    cat squid_access.log | awk '{print $3}' | sort | uniq       //Should sort through IPs 
    cat squid_access.log | awk '{print $6}' | sort | uniq –c    //Should sort through all HTTP methods

    Note: This commands may need to edited for different lines/values.
    This is just what I found that worked.

sqlite:
    The NGL says to use SQLPro if you have OSX, however I found that using DB Browser for SQLite works just as well on Linux.
    Best advice on how to answer these questions is to find the section of the database that hase all the urls, 
    and then simply search through them till you find the informatino the qustion is looking for.
    
    Note: You may have to open some urls to find relevant inforamtion.