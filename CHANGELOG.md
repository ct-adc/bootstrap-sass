## 更新日志

### 1.0.3

*2018-02-05*

- 修复 modal-dialog中因修复v1.0.2#2时引起的动画不自然的情况.方案为:

```
.modal.in .modal-dialog, .modal.fade .modal-dialog{
  -webkit-transition: initial;
  -moz-transition: initial;
  -o-transition: initial;
  transition: initial;
}

```

### 1.0.2

*2017-12-01*

- 修复 添加form-group样式，和栅格化的padding对应，防止同样的同样的1份栅格长度不一致,如col-sm-4中的col-sm-2 和col-sm-8中的col-sm-1
```
.form-horizontal .form-group{
    margin-left: -5px;
    margin-right: -5px;
}
```

- 修复 modal-dialog中因为内容突然变高（如日期弹窗），超出部分导致弹框整体高度变高，有可能出现的bug：
刚开始弹窗不够高，所以没有在遮罩层中滚动，但如日期的弹层多出的部分超出了弹框，导致遮罩层显示出了滚动条。
那么表现出来就是弹框会左右摆动。

### 1.0.1

**2017-09-07**

- 优化 新增red类，修改well-sm的margin-bottom


### 1.0.0 发布

**2017-07-30**

- 添加
```
[v-cloak] {display: none; }
.container-fluid{
padding-top:5px;
}
```



