# DOM_tree
dom树_删除，添加，修改


  1：这个有删除，添加，修改，功能
  
  
    json文件： text.json文件
                            [
                            {
                                "id": 1,
                                "pId": 0,
                                "name": "湖北省",
                                "open": true
                            },
                            {
                                "id": 11,
                                "pId": 1,
                                "name": "武汉市",
                                "open": true
                            },
                            {
                                "id": 111,
                                "pId": 11,
                                "name": "汉口"
                            },
                            {
                                "id": 112,
                                "pId": 11,
                                "name": "汉阳"
                            },
                            {
                                "id": 113,
                                "pId": 11,
                                "name": "武昌"
                            },
                            {
                                "id": 12,
                                "pId": 1,
                                "name": "黄石市"
                            },
                            {
                                "id": 121,
                                "pId": 12,
                                "name": "黄石港区"
                            },
                            {
                                "id": 122,
                                "pId": 12,
                                "name": "西塞山区"
                            },
                            {
                                "id": 123,
                                "pId": 12,
                                "name": "下陆区"
                            },
                            {
                                "id": 124,
                                "pId": 12,
                                "name": "铁山区"
                            },
                            {
                                "id": 13,
                                "pId": 1,
                                "name": "黄冈市"
                            },
                            {
                                "id": 2,
                                "pId": 0,
                                "name": "湖南省",
                                "open": true
                            },
                            {
                                "id": 21,
                                "pId": 2,
                                "name": "长沙市",
                                "open": true
                            },
                            {
                                "id": 211,
                                "pId": 21,
                                "name": "芙蓉区"
                            },
                            {
                                "id": 212,
                                "pId": 21,
                                "name": "天心区"
                            },
                            {
                                "id": 213,
                                "pId": 21,
                                "name": "岳麓区"
                            },
                            {
                                "id": 214,
                                "pId": 21,
                                "name": "开福区"
                            },
                            {
                                "id": 22,
                                "pId": 2,
                                "name": "株洲市"
                            },
                            {
                                "id": 221,
                                "pId": 22,
                                "name": "天元区"
                            },
                            {
                                "id": 222,
                                "pId": 22,
                                "name": "荷塘区"
                            },
                            {
                                "id": 223,
                                "pId": 22,
                                "name": "芦淞区"
                            },
                            {
                                "id": 224,
                                "pId": 22,
                                "name": "石峰区"
                            },
                            {
                                "id": 23,
                                "pId": 2,
                                "name": "湘潭市"
                            },
                            {
                                "id": 231,
                                "pId": 23,
                                "name": "雨湖区"
                            },
                            {
                                "id": 232,
                                "pId": 23,
                                "name": "岳塘区"
                            },
                            {
                                "id": 233,
                                "pId": 23,
                                "name": "湘乡市"
                            },
                            {
                                "id": 234,
                                "pId": 23,
                                "name": "韶山市"
                            },
                            {
                                "id": 3,
                                "pId": 0,
                                "name": "湖南省",
                                "open": true
                            },
                            {
                                "id": 31,
                                "pId": 3,
                                "name": "长沙市",
                                "open": true
                            },
                            {
                                "id": 311,
                                "pId": 31,
                                "name": "芙蓉区"
                            },
                            {
                                "id": 312,
                                "pId": 31,
                                "name": "天心区"
                            },
                            {
                                "id": 313,
                                "pId": 31,
                                "name": "岳麓区"
                            },
                            {
                                "id": 314,
                                "pId": 31,
                                "name": "开福区"
                            },
                            {
                                "id": 32,
                                "pId": 3,
                                "name": "株洲市"
                            },
                            {
                                "id": 321,
                                "pId": 32,
                                "name": "天元区"
                            },
                            {
                                "id": 322,
                                "pId": 32,
                                "name": "荷塘区"
                            },
                            {
                                "id": 323,
                                "pId": 32,
                                "name": "芦淞区"
                            },
                            {
                                "id": 324,
                                "pId": 32,
                                "name": "石峰区"
                            },
                            {
                                "id": 33,
                                "pId": 3,
                                "name": "湘潭市"
                            },
                            {
                                "id": 331,
                                "pId": 33,
                                "name": "雨湖区"
                            },
                            {
                                "id": 332,
                                "pId": 33,
                                "name": "岳塘区"
                            },
                            {
                                "id": 333,
                                "pId": 33,
                                "name": "湘乡市"
                            },
                            {
                                "id": 334,
                                "pId": 33,
                                "name": "韶山市"
                            }
                        ]


   index.html文件
   
        <link href="metroStyle/metroStyle.css" type="text/css" rel="stylesheet">
        <script src="js/jquery-1.4.4.min.js"></script>
        <script src="js/jquery.ztree.all.min.js"></script>
        <script src="js/jquery.ztree.core.min.js"></script>
        <script src="js/jquery.ztree.excheck.min.js"></script>
        <script src="js/jquery.ztree.exedit.min.js"></script>
        <script src="js/jquery.ztree.exhide.min.js"></script>

        <div class="content_wrap">
            <div class="zTreeDemoBackground left" style="text-align: center;">
                <ul id="baseTree" class="ztree" style="height: 300px; width:200px; overflow-y: auto"></ul>
            </div>
        </div>

       <script type="text/javascript">
      // 增加ztree节点
        var setting = {
            view: {
                addHoverDom: addHoverDom, //当鼠标移动到节点上时，显示用户自定义控件
                removeHoverDom: removeHoverDom, //离开节点时的操作
                //fontCss: getFontCss //个性化样式
            },
            edit: {
                enable: true, //单独设置为true时，可加载修改、删除图标
                editNameSelectAll: true,
                //showRemoveBtn: showRemoveBtn,
               // showRenameBtn: showRenameBtn
            },
            data: {
                simpleData: {
                    enable: true,
                    idKey: "id",
                    pIdKey: "pId",
                    system:"system",
                    rootPId: ""
                }
            },
            callback: {
                //onClick: zTreeOnClick, //单击事件
                onRemove: onRemove, //移除事件
                onRename: onRename //修改事件
             }
           };

        $(document).ready(function(){
             $.get('text.json',function(data){
                var zNodes=data;
                //console.log(datatext);
             $.fn.zTree.init($("#baseTree"), setting, zNodes);
            })

        });
        function addHoverDom(treeId, treeNode) {
            var sObj = $("#" + treeNode.tId + "_span"); //获取节点信息
            if (treeNode.editNameFlag || $("#addBtn_"+treeNode.tId).length>0)
                         return;
            //定义添加按钮
            var addStr = "<span class='button add' id='addBtn_" + treeNode.tId + "' title='add node' onfocus='this.blur();'></span>";
            //加载添加按钮
            sObj.after(addStr);
            var btn = $("#addBtn_"+treeNode.tId);
            //绑定添加事件，并定义添加操作
            if (btn) btn.bind("click", function(){
                var zTree = $.fn.zTree.getZTreeObj("tree");
                //将新节点添加到数据库中
                var name='NewNode';
                $.post('./index.php?r=data/addtree&pid='+treeNode.id+'&name='+name,function (data) {
                    //获取新添加的节点Id
                    var newID = data;
                    //页面上添加节点
                    zTree.addNodes(treeNode, {id:newID, pId:treeNode.id, name:name});
                    //根据新的id找到新添加的节点
                    var node = zTree.getNodeByParam("id", newID, null);
                    //让新添加的节点处于选中状态
                    zTree.selectNode(node);
                });
            });
        };

        function removeHoverDom(treeId, treeNode) {
            $("#addBtn_"+treeNode.tId).unbind().remove();
        };
        //修改节点
        function onRename(e, treeId, treeNode, isCancel) {
            //  console.log(treeNode.id)
            // console.log(treeNode.name)
            //需要对名字做判定的，可以来这里写~~
            $.post('./index.php?r=data/modifyname&id='+treeNode.id+'&name='+treeNode.name);
        }

    // 修改节回调
        function beforeRename(treeId, treeNode, newName, isCancel) {
            if (newName.length == 0) {
                alert("节点名称不能为空.");
                return false;
            }
            return true;
        }

        //删除节点
        function onRemove(e, treeId, treeNode) {
          //  console.log(treeNode.id);
            //需要对删除做判定或者其它操作，在这里写~~
            $.post('./index.php?r=data/del&id='+treeNode.id);
        }
        //删除节点回调
        function beforeRemove(treeId, treeNode) {
            var zTree = $.fn.zTree.getZTreeObj("tree");
            zTree.selectNode(treeNode);
            return confirm("确认删除 节点 -- " + treeNode.name + " 吗？");
        }
    </script>



2：单纯dom树 ：
      

                      <!--<link href="zTreeStyle/zTreeStyle.css" type="text/css" rel="stylesheet"/>-->
                      <link href="metroStyle/metroStyle.css"  type="text/css" rel="stylesheet">
                      <script src="js/jquery-1.4.4.min.js"></script>
                      <script src="js/jquery.ztree.all.min.js"></script>
                      <script src="js/jquery.ztree.core.min.js"></script>
                      <script src="js/jquery.ztree.excheck.min.js"></script>
                      <script src="js/jquery.ztree.exedit.min.js"></script>
                      <script src="js/jquery.ztree.exhide.min.js"></script>

                    <div class="content_wrap">
                        <div class="zTreeDemoBackground left" style="text-align: center;">
                            <ul id="baseTree" class="ztree" style="height: 300px; width:200px; overflow-y: auto"></ul>
                            <input type="button" id="btn" onclick="removeNodes()" value="删除节点"/>
                        </div>
                    </div>

                      <script type="text/javascript">

                          var setting = {

                              data: {
                                  simpleData: {
                                      enable: true
                                  }
                              }

                          };
                          var zNodes =[
                              { id:1, pId:0, name:"湖北省", open:true},
                              { id:11, pId:1, name:"武汉市", open:true},
                              { id:111, pId:11, name:"汉口"},
                              { id:112, pId:11, name:"汉阳"},
                              { id:113, pId:11, name:"武昌"},
                              { id:12, pId:1, name:"黄石市"},
                              { id:121, pId:12, name:"黄石港区"},
                              { id:122, pId:12, name:"西塞山区"},
                              { id:123, pId:12, name:"下陆区"},
                              { id:124, pId:12, name:"铁山区"},
                              { id:13, pId:1, name:"黄冈市"},
                              { id:2, pId:0, name:"湖南省", open:true},
                              { id:21, pId:2, name:"长沙市", open:true},
                              { id:211, pId:21, name:"芙蓉区"},
                              { id:212, pId:21, name:"天心区"},
                              { id:213, pId:21, name:"岳麓区"},
                              { id:214, pId:21, name:"开福区"},
                              { id:22, pId:2, name:"株洲市"},
                              { id:221, pId:22, name:"天元区"},
                              { id:222, pId:22, name:"荷塘区"},
                              { id:223, pId:22, name:"芦淞区"},
                              { id:224, pId:22, name:"石峰区"},
                              { id:23, pId:2, name:"湘潭市"},
                              { id:231, pId:23, name:"雨湖区"},
                              { id:232, pId:23, name:"岳塘区"},
                              { id:233, pId:23, name:"湘乡市"},
                              { id:234, pId:23, name:"韶山市"}
                          ];

                          $(document).ready(function(){
                              $.fn.zTree.init($("#baseTree"), setting, zNodes);
                          });

                          /**
                           * 删除选中节点
                           */
                          function removeNodes()
                          {
                              var treeObj = $.fn.zTree.getZTreeObj("baseTree");
                              //选中节点
                              var nodes = treeObj.getSelectedNodes();
                              for (var i=0, l=nodes.length; i < l; i++)
                              {
                                  //删除选中的节点
                                  treeObj.removeNode(nodes[i]);
                              }
                          }

                      </script>







