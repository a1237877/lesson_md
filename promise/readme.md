**24岁了，在杭州有一个可爱的女朋友
**的女朋友是个童养媳
** 的女朋友想跟 ** 结婚
可是**的女朋友才18岁，还没到法定年龄
** 女朋友天天羡慕着别人有情人终成眷属的生活
时不时的跟 ** 腻歪
** 下定决心要娶自己的女朋友
于是，有一天，** 跟远在老家的女朋友打电话，作出一个承诺：“再过两年，等你到了法定结婚年纪，我就带你去领证”
女朋友感动不已，约了**工作之余要记得来看自己

为了这个承诺，** 努力工作，同时也在静候时间的到来

# .then(fun)
.then 接收的就是一个回调函数，跟setTimeout一样，只需要写函数名，就相当于把整个函数题放进去调用

# .all([a, b, c])
.all 里面没有排序，放在.all里面的函数都是一起执行的，至于先执行完哪一个，就看哪一个耗时少了，
而.all 后面接的 .then 需要等 .all 里面的函数全部执行完才能执行

# .race([a, b])
有些时候，多个异步任务是为了容错。比如，同时向两个URL读取用户的个人信息，只需要获得先返回的结果即可
函数 a 和 函数 b 是在干同样一件事，（比如都是去接口请求数据，这两个请求的接口不一样，需要的时间也不一样），那么谁先请求到我要的数据，我就用谁的数据，反应慢的函数也会执行，只是，返回的的值，我们不需要了