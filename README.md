## Написання плагіну kubectl та його використання

1. створимо файл цим кодом плагіну
   
```touch kubeplugin```

2. надамо права на виконання  
   
```chmod 755 kubeplugin```
 
3. копіюємо плагін у системну директорію
   
```sudo cp ./kubeplugin /usr/local/bin/kubectl-kubeplugin```

4. перевіримо коректність встановлення плагіну

```kubectl plugin list```

The following compatible plugins are available:
/root/.krew/bin/kubectl-krew
/root/.krew/bin/kubectl-ns
/usr/local/bin/kubectl-kubeplugin

5. Перевіримо роботу плагіну:

```k kubeplugin node kube-system```

```k kubeplugin pod kube-system```

![Task9_kubeplugin_output](https://github.com/sbazanov/Task9_k8s_ktop/assets/96147501/985d191a-bcfc-40ad-a25a-851439f96585)
