#UIAlertController and UIAlertAction in IOS 8

1. Create an instance of UIAlertController with class method `alertControllerWithTitle: message: preferredStyle:`.

       UIAlertController *alert = [UIAlertController alertControllerWithTitle:@"Selected name" message:rowString preferredStyle:UIAlertControllerStyleAlert];
	
2. Create an instance of UIAlertAction with class method `actionWithTitle: style: handler:`.
            
       UIAlertAction *info = [UIAlertAction actionWithTitle:@"OK" style:UIAlertActionStyleDefault handler:^(UIAlertAction *action) {
        //do nothing
        }];
3. Add `info` object to `alert`.

       [alert addAction:info]; 
       
4. Add `alert` to current ***ViewController***.

		[self presentViewController:alert animated:YES completion:nil];
		
  ![MouController icon](./resources/20150302/alertcontroller.png)
