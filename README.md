# RasaChatBot-en
基于RASA3.0+搭建的英文对话系统，适合初学者入门

# procedure
1. rasa data validate

        用法: rasa data validate [-h] [-v] [-vv] [--quiet] [-d DOMAIN] [--data DATA]
        
        可选参数: 
         -h, --help     显示帮助消息并退出。
         -d DOMAIN, --domain DOMAIN
                        域规范(yml文件)。(默认:domain.yml)
        --data DATA     包含Rasa数据的文件或目录。(默认:data)  
        
        Python日志选项:
         -v, --verbose  详细输出。将日志记录级别设置为INFO。(默认:None)
         -vv, --debug   打印大量的调试语句。设置日志记录级别为 DEBUG。(默认:None)
         --quiet        将日志记录级别设置为WARNING。(默认:None)

2. rasa train (train both nlu and core)  
3. rasa run actions (optional) if you redefined actions, 
4. rasa run -m models --endpoints endpoints.yml (run the rasa bot)  
5. rasa shell (interactive with chat bot) ([/stop] to exit)
6. rasa evaluate markers all out.csv (evaluate chat bot) 