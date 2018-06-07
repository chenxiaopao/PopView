# PopView
模仿今日头条上的PopView

Usage

    var firstPopView : PopView!
    let imageNames = ["add_textpage_night_17x12_","add_textpage_night_17x12_","add_textpage_night_17x12_","add_textpage_night_17x12_"]
    let titleNames = ["发图文","拍小视频","上传视频","提问"]
    let size = CGSize(width: 130, height: 150)
    firstPopView = PopView(popViewSize:size
        , arrowPoint: CGPoint(x:110,y:100),arrowSize:CGSize(width:10,height:20), titleNames:titleNames , imageNames: imageNames)
    firstPopView.delegate = self
    view.addSubview(firstPopView)
