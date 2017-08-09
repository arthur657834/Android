滑动解锁:
smile = TouchAction(self.driver)
smile.press(x=wm['width']/2, y=wm['height']*3/4).move_to(x=0, y=wm['height']/4).release().perform()

九宫格解锁:
场景1:
九宫格的每一格组成一个list，通过一下方法取得
list_pwd = self.driver.find_elements_by_class_name("android.view.View")
for lj in list_pwd:
    print lj
TouchAction(self.driver).press(list_pwd[0]).move_to(list_pwd[0]).move_to(list_pwd[2]).wait(100).move_to(list_pwd[5]).release().perform()

场景2:
smile.press(x=100, y=370).move_to(x=0, y=130).move_to(x=0, y=130) \
.move_to(x=130, y=0).move_to(x=130, y=0).move_to(x=0, y=-130).wait(5000) \
.release().perform()

负数是向上
