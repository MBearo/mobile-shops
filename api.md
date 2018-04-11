> 所有变量命名遵循 驼峰命名 如: img nickName forgetMyHomework
> 全用post就行了，区别了
> 接口里上面是我请求的，下面的是返回给我的
## 移动端展示的就是用户用的
### 登录 login
```
{
    phone:'',
    password:''
    
}
```
```
{
    msg:'',
    errorcode:'',
    data:{
        id:'',
    }
    
}
```
之后的接口我就不写那个msg errorcode了 都要带着
### 注册 register
```
{
    phone:'',
    password:''
    name:''
}

```
```
{
    msg:'',
    errorcode:'',
    data:{
       
    }
}
```
返回data为空的话这样就好了
### 拉取个人信息 userData
```
{
    id:''
}
```
```
{
    name:'',
    img:'',//头像
    like:[{  //喜欢的文章列表
        id:''//文章的id
    }],
    attention:[{ //关注的发布文章的人
        id:'' //管理员id
    }],
    buy:[{ //购买的文章id
        id:'' //文章id
    }]
}
```
### 拉取管理员信息 adminData
```
{
    id:''
}
```
```
{
    name:'',
    img:'',//头像
    article:[{ //发布的文章
        id:'' //文章的id
    }],
    attentionUser:[{ //关注这个管理员的用户
        id:'' //用户的id
    }]
}
```
### 拉取文章详情 articleData
```
{
    id:''
}
```
```
{
    id:'',//管理员id
    title:'',
    img:'',//banner图
    like:[{
        id:'' //喜欢的人的id
    }]
}
```
### 拉取管理员列表 adminList
 ```
    不传参
 ```
 ```
    
 ```