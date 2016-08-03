# RadioAndCheck
  原来使用OC为公司开发了一整套的单选、多选、填空、简单、查看试题答案、查看试题解析等一整套的在线考试、在线练习框架，功能较为复杂，近日有朋友要用到的单选、多选按钮，就抽时间从原来框架中提取出来一部分代码，组成一套新的简洁版的单选、多选库，方便使用。只使用单选可以不导入多选库，两个不互相依存，但是都依赖MineLibry文件。觉得不错记得赞一下哦！

####效果展示

![image](https://github.com/SZLCode/RadioAndCheck/raw/master/radio.gif)


![image](https://github.com/SZLCode/RadioAndCheck/raw/master/check.gif)


####单选按钮使用教程
        RadioButton *radioButton = [[RadioButton alloc]initWithFrame:CGRectMake(0, 60, 414, 736)];
        radioButton.delegate = self;
        radioButton = [radioButton initRadioButtonTitle:@"请评价好坏" selectImgName:nil unselectImgName:nil labelArr:@[@"好",@"BBBBBBBBBBBBBBBBBBBBB",@"这是第三个选项，这是第三个选项，你看我可以自动换行哟！不信吗？看我换行给你看！"]];
    
        [self.view addSubview:radioButton];
        
        
####多选按钮使用教程
    CheckButton *checkBtn = [[CheckButton alloc]initWithFrame:CGRectMake(0, 20, 414, 736)];
    checkBtn.delegate = self;
    checkBtn = [checkBtn initCheckButtonTitle:nil selectImgName:nil unselectImgName:nil labelArr:@[@"AAAAAAAAAAAAAAAAAAA",@"BBBBBBBBBBBBB",@"这个是多选项哦，这个是多选项哦，多选项哦，选项哦，项哦，哦！",@"DDDDDDDDDDDDDDD",@"EEEEEEEEEEEEEE",@"这个是最后一项，我可以继续增加很多选项哦，不信你可以增加GGGGGGGGGGGG来试一下哦！"]];
