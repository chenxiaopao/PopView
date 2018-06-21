
# PopView
模仿今日头条上的PopView,直接拖到项目中即可使用

用法：

    var firstPopView : PopView!
    let imageNames = ["add_textpage_night_17x12_","add_textpage_night_17x12_","add_textpage_night_17x12_","add_textpage_night_17x12_"]
    let titleNames = ["发图文","拍小视频","上传视频","提问"]
    let size = CGSize(width: 130, height: 150)
    firstPopView = PopView(popViewSize:size
        , arrowPoint: CGPoint(x:110,y:100),arrowSize:CGSize(width:10,height:20), titleNames:titleNames , imageNames: imageNames)
    firstPopView.delegate = self
    view.addSubview(firstPopView)
    
    遵守代理方法
    extension ViewController:PopViewDelegate{
        func popView(_ popViewCellBtn: UIButton, popTag: Int) {
        //通过添加的项由Button.tag区分，从0开始，
            let index = popViewCellBtn.tag
            switch index{
            case 0:
                print(titleNames[index])
                break
            case 1:
                print(titleNames[index])
                break
            case 2:
                print(titleNames[index])
                break
            case 3:
                print(titleNames[index])
                break
            default:
                break
            }
        }
    }


![](https://github.com/chenxiaopao/PopView/blob/master/CB114982-81A0-4C3E-990D-E9874A875F01.png)
