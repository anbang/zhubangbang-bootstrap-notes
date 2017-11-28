说明：如果你使用导航来制作一个导航栏，请确保向<ul>的逻辑父元素添加了role="navigation"或者给整个导航条包裹一个<nav>元素。
不要在<ul>的本身上面添加navigation，因为这将阻止它被使用辅助技术的用户声明为一个真正的列表。

disabled放在链接、按钮、checkbox、testarea等都是不可操作的意思；

### nav的class名

** 基础类名 **
- nav
- nav-item

** nav级的扩展、放在nav这级 **
- nav-tabs 		改为选项卡格式的导航
- nav-pills		改为丸状导航
- nav-stacked	只需要向.nav.nav-pills添加.nav-stacked类就可以做堆叠丸状导航，这个类名4.0.0beta2版本没有；










### 弹出菜单

- dropdown
	- dropdown-toggle
	- dropdown-menu
		- dropdown-item
		- dropdown-divider