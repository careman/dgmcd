title: 常平装修，到常平福易买不锈钢门，
keywords: 常平不锈钢门,常平不锈钢门厂家,常平塑钢门,常平家装房间门,常平 室内门,常平办公室门,常平不锈钢门报价,常平楼梯扶手,常平防护网，常平实木门,常平防盗门,常平安全门,常平防火门,东莞不锈钢门，东莞不锈钢门公司，东莞不锈钢门工厂，东莞不锈钢门企业，东莞不锈钢门供应商
description: 常平装修门窗请直接联系我们，电话13715281934，谢岗福易门业主营：不锈钢四开门,不锈钢别墅门,不锈钢楼宇对讲门,实木门，防火门，自动门。我们是品牌不锈钢门厂家直销店，为企业装修和家庭装修提供最优惠的价格和最优质的服务
---
常平有很多建材城？
常平也有很多门窗店？
常平到谢岗不方便？
但是你知不知道，做企业都是要赚钱的！
但是你知不知道，常平的房租比谢岗贵！
但是你知不知道，建材城的租金比独立店铺贵的不止两三倍！

还有你更不知道的，我们是免费上门测量，免费送货上门，更重要的是我们免费给安装，所有产品包安装。

所以，我问你，你为什么不早点来我们谢岗福易买不锈钢门，铝合金门、实木门，安全防护网，你想要的门窗产品我们都有哟。
是的，我们就在你的身边哦。
对的，常平装修买门窗请直接联系品牌不锈钢门常平业务经理，电话13715281934，联系人：老表



是不是，正好你需要，我们也专业。
记得，品牌门窗哦，记得厂家直销哦。
主营产品：不锈钢单开门，不锈钢门双开门，不锈钢防火门，实木门，办公室门，防护网，楼梯扶手，铝合金拖拉门，铝合金防护栏等等门窗及安全防护产品，产品质量好，安全有保障。


  <!--百度地图容器-->
  <div style="width:697px;height:550px;border:#ccc solid 1px;" id="dituContent"></div>
</body>
<script type="text/javascript">
    //创建和初始化地图函数：
    function initMap(){
        createMap();//创建地图
        setMapEvent();//设置地图事件
        addMapControl();//向地图添加控件
        addMarker();//向地图中添加marker
        addRemark();//向地图中添加文字标注
    }
    
    //创建地图函数：
    function createMap(){
        var map = new BMap.Map("dituContent");//在百度地图容器中创建一个地图
        var point = new BMap.Point(114.142807,22.968764);//定义一个中心点坐标
        map.centerAndZoom(point,18);//设定地图的中心点和坐标并将地图显示在地图容器中
        window.map = map;//将map变量存储在全局
    }
    
    //地图事件设置函数：
    function setMapEvent(){
        map.enableDragging();//启用地图拖拽事件，默认启用(可不写)
        map.enableScrollWheelZoom();//启用地图滚轮放大缩小
        map.enableDoubleClickZoom();//启用鼠标双击放大，默认启用(可不写)
        map.enableKeyboard();//启用键盘上下左右键移动地图
    }
    
    //地图控件添加函数：
    function addMapControl(){
        //向地图中添加缩放控件
	var ctrl_nav = new BMap.NavigationControl({anchor:BMAP_ANCHOR_TOP_LEFT,type:BMAP_NAVIGATION_CONTROL_LARGE});
	map.addControl(ctrl_nav);
        //向地图中添加缩略图控件
	var ctrl_ove = new BMap.OverviewMapControl({anchor:BMAP_ANCHOR_BOTTOM_RIGHT,isOpen:1});
	map.addControl(ctrl_ove);
        //向地图中添加比例尺控件
	var ctrl_sca = new BMap.ScaleControl({anchor:BMAP_ANCHOR_BOTTOM_LEFT});
	map.addControl(ctrl_sca);
    }
    
    //标注点数组
    var markerArr = [{title:"谢岗福易门业",content:"谢岗福易门业，不锈钢门，防火门，室内门，卫生间门，厨房门，实木门。",point:"114.143099|22.968447",isOpen:0,icon:{w:21,h:21,l:0,t:0,x:6,lb:5}}
		 ];
    //创建marker
    function addMarker(){
        for(var i=0;i<markerArr.length;i++){
            var json = markerArr[i];
            var p0 = json.point.split("|")[0];
            var p1 = json.point.split("|")[1];
            var point = new BMap.Point(p0,p1);
			var iconImg = createIcon(json.icon);
            var marker = new BMap.Marker(point,{icon:iconImg});
			var iw = createInfoWindow(i);
			var label = new BMap.Label(json.title,{"offset":new BMap.Size(json.icon.lb-json.icon.x+10,-20)});
			marker.setLabel(label);
            map.addOverlay(marker);
            label.setStyle({
                        borderColor:"#808080",
                        color:"#333",
                        cursor:"pointer"
            });
			
			(function(){
				var index = i;
				var _iw = createInfoWindow(i);
				var _marker = marker;
				_marker.addEventListener("click",function(){
				    this.openInfoWindow(_iw);
			    });
			    _iw.addEventListener("open",function(){
				    _marker.getLabel().hide();
			    })
			    _iw.addEventListener("close",function(){
				    _marker.getLabel().show();
			    })
				label.addEventListener("click",function(){
				    _marker.openInfoWindow(_iw);
			    })
				if(!!json.isOpen){
					label.hide();
					_marker.openInfoWindow(_iw);
				}
			})()
        }
    }
    //创建InfoWindow
    function createInfoWindow(i){
        var json = markerArr[i];
        var iw = new BMap.InfoWindow("<b class='iw_poi_title' title='" + json.title + "'>" + json.title + "</b><div class='iw_poi_content'>"+json.content+"</div>");
        return iw;
    }
    //创建一个Icon
    function createIcon(json){
        var icon = new BMap.Icon("http://app.baidu.com/map/images/us_mk_icon.png", new BMap.Size(json.w,json.h),{imageOffset: new BMap.Size(-json.l,-json.t),infoWindowOffset:new BMap.Size(json.lb+5,1),offset:new BMap.Size(json.x,json.h)})
        return icon;
    }
//文字标注数组
    var lbPoints = [{point:"114.143144|22.968381",content:"福易门业产品：不锈钢门，防火门，实木门，塑钢门，安全门，厨房门，洗手间门，"}
		 ];
    //向地图中添加文字标注函数
    function addRemark(){
        for(var i=0;i<lbPoints.length;i++){
            var json = lbPoints[i];
            var p1 = json.point.split("|")[0];
            var p2 = json.point.split("|")[1];
            var label = new BMap.Label("<div style='padding:2px;'>"+json.content+"</div>",{point:new BMap.Point(p1,p2),offset:new BMap.Size(3,-6)});
            map.addOverlay(label);
            label.setStyle({borderColor:"#999"});
        }
    }
    
    initMap();//创建和初始化地图
</script>
