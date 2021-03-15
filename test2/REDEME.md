# 第一次实验
## 18软件3班 赵张阳 201810414329

![](png2.png)
![](png1.png)

我认为最简洁的语句

SELECT d.department_name,count(e.job_id)as "部门总人数",
avg(e.salary)as "平均工资"
from hr.departments d JOIN hr.employees e
on d.department_id = e.department_id
and d.department_name in ('IT','Sales')
GROUP BY d.department_name;