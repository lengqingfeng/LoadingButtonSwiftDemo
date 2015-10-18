# LoadingButtonSwiftDemo
Like Zhifubao PayButton Animation 
> 
Animation like down gif
>
![ ](http://ww3.sinaimg.cn/mw690/b383e575gw1ex5pehic8pg20hs0qoth4.gif)
![ ](http://ww2.sinaimg.cn/mw690/b383e575gw1ex5pe7pp2ug20hs0qodos.gif)
>
USE
------- 
       
        loadingView =   LoadingButtonSwift(fram: CGRectMake((self.view.frame.size.width/2)-90, 100, 180, 44), title: "确定", backColor:UIColorFromRGB(0x1487de))
        
        loadingView!.startGetHttpData = {
            
            print("start http data")
            self.performSelector("success", withObject: self, afterDelay: 1)
       }
        
        loadingView?.getDataSuccessClosures = {
            
            print("success  push")
            
        }
        loadingView?.getDataErrorClosures = {
            
           print("error")
        }
        self.view.addSubview(loadingView!)
[Thanks  MMMaterialDesignSpinner](https://github.com/misterwell/MMMaterialDesignSpinner)<br /> 
