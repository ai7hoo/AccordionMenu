# AccordionMenu
无限级别的竖向折叠菜单
依赖jquery

```` javascript
<script>
  var testMenu = [
	{
	  "name": "一级菜单",
	  "submenu": [
		{
		  "name": "二级菜单",
		  "url": "#/list-a"
		},
		{
		  "name": "二级菜单",
		  "url": ""
		}
	  ]
	},
	{
	  "name": "一级菜单",
	  "submenu": [
		{
		  "name": "二级菜单",
		  "url": ""
		},
		{
		  "name": "二级菜单",
		  "submenu": [
			{
			  "name": "三级菜单",
			  "submenu": [
				{
				  "name": "四级菜单",
				  "url": ""
				}
			  ]
			},
			{
			  "name": "三级菜单",
			  "url": ""
			}
		  ]
		},
		{
		  "name": "二级菜单",
		  "url": ""
		},
		{
		  "name": "二级菜单",
		  "submenu": [
			{
			  "name": "三级菜单",
			  "submenu": [
				{
				  "name": "四级菜单",
				  "url": ""
				},
				{
				  "name": "四级菜单",
				  "submenu": [
					{
					  "name": "五级菜单",
					  "url": ""
					},
					{
					  "name": "五级菜单",
					  "url": ""
					}
				  ]
				}
			  ]
			},
			{
			  "name": "三级菜单",
			  "url": ""
			}
		  ]
		},
		{
		  "name": "二级菜单",
		  "url": ""
		}
	  ]
	},
	{
	  "name": "一级菜单",
	  "submenu": [
		{
		  "name": "二级菜单",
		  "url": ""
		},
		{
		  "name": "二级菜单",
		  "url": ""
		},
		{
		  "name": "二级菜单",
		  "url": ""
		}
	  ]
	}
  ];
  new AccordionMenu({
    menuArrs:testMenu,//  JSON 数据格式的菜单
    containerCls:'.wrap-menu',  //  外部容器，默认 .wrap-menu
    type:'click', // 默认为 click，也可以是 mouseover
    renderCallBack:null,  // 渲染完成 HTML 结构后的回调
    clickItemCallBack:null, // 每点击一次的回调
  });
</script>
