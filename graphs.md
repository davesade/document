## Inserting graphs into my document

This I would consider as *slightly* advanced, because now we leave comfortable environment of MarkDown syntax. The tool we use is called [Docsify](https://docsify.js.org/#/) and it does support numerous plugins. Here I'm using simple plugin called [Docsify echarts plugin](https://github.com/xiguaxigua/docsify-echarts-plugin). It's not so hard to implement it (have a look at *index.html* file, where scripts are defined).  
Result could then look like this:  

```chart
{
  settings: {
    theme: {
      categoryAxis: {
        axisLine: { show: false },
        axisTick: { show: false },
        splitLine: { show: false }
      },
      valueAxis: { axisLine: { show: false } }
    }
  },
  xAxis : [
    {
      type : 'category',
      data : ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
    }
  ],
  yAxis : [{ type : 'value' }],
  series : [
    {
      name:'直接访问',
      type:'bar',
      barWidth: '60%',
      data:[10, 52, 200, 334, 390, 330, 220]
    }
  ]
}
```

In the repository, have a look at file *graphs.md*, you will see, that actual graphs is saved in JSON format. That is beyond MarkDown knowledge, but it's good to know about it, right?  
