这是一个标题切换的View，你可以把这个View添加到控制器里面当标题切换器。

可以在Demo里面看到，用这个View只需要四个步骤：

1，初始化

self.switchView = [[CommonSwitchControl alloc] initWithFrame:CGRectMake(0, 0, width, 66)];

2，传入标题列表，标题个数，下划线的长度

self.switchView.buttonNumber = 2;
self.switchView.buttonTitles = @[@"会员统计",@"您的设置"];
self.switchView.underLineW = 80;

3，初始化View

[self.switchView initView];

4，实现Delegate

- (void)switchButton:(NSInteger )buttonNumber{
    NSLog(@"您选中了%ld",buttonNumber);
}

很简单的，一看就会用。


