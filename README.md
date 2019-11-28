# Group-Project
By Michael Chen, Zhangpeng, Su Hongyang
[http://michaelisawesome.epizy.com/Group-Project.html](http://michaelisawesome.epizy.com/Group-Project.html)

![plan.png](plan.png)
We find the highest participation rate of 2012 and 2013.
```{r}
pr2012_highest <- sat %>%
    filter(part_rate ==100, year == 2012) %>%
    select(District) 
ggplot(pr2012_highest) +
  geom_bar(aes(District))+
coord_flip()
```

```{r}
pr2013_highest <- sat %>%
    filter(Part_rate_2013 == 100, year == 2013) %>%
    select(District) 
ggplot(pr2013_highest) +
  geom_bar(aes(District))+
coord_flip()
```
