# lecture_50_JS_Interface_Events_Pointer_events  
# lecture_51_JS_Interface_Events_Scrolling  

#  [Задачи ](https://github.com/schoolteacherMP/lecture_50_JS_Interface_Events_Pointer_events/blob/main/tasks.md)  

События указателя позволяют одновременно обрабатывать действия с помощью мыши, касания и пера, в едином фрагменте кода.  

События указателя расширяют события мыши. Мы можем заменить mouse на pointer в названиях событий и код продолжит работать для мыши, при этом получив лучшую поддержку других типов устройств.  

При обработке переносов и сложных касаний, которые браузер может попытаться обработать сам, не забывайте отменять действие браузера и ставить touch-action: none в CSS для элементов, с которыми мы взаимодействуем.  

Дополнительные возможности событий указателя:  

- Поддержка мультитач с помощью pointerId и isPrimary.  
- Особые свойства для определённых устройств, такие как pressure, width/height и другие.  
- Захват указателя: мы можем перенаправить все события указателя на определённый элемент до наступления события pointerup/pointercancel.  

На данный момент события указателя поддерживаются в основных браузерах, поэтому мы можем безопасно переходить на них, особенно если нет необходимости в поддержке IE10 и Safari 12. И даже для этих браузеров есть полифилы, которые добавляют эту поддержку.
