//
//  ViewController.swift
//  ChineseZodiac
//
//  Created by Daniel Yao on 3/19/15.
//  Copyright (c) 2015 Daniel Yao. All rights reserved.
//

import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var yearOfBirth: UITextField!
    @IBOutlet weak var image: UIImageView!
    
    let offset = 4
//    
//    override func viewDidLoad() {
//        super.viewDidLoad()
//        // Do any additional setup after loading the view, typically from a nib.
//    }
//
//    override func didReceiveMemoryWarning() {
//        super.didReceiveMemoryWarning()
//        // Dispose of any resources that can be recreated.
//    }
    
    override func touchesEnded(touches: NSSet, withEvent event: UIEvent) {
        yearOfBirth.resignFirstResponder()
        // when touch the white space, the keypad will disappear
    }

    @IBAction func okTapped(sender: AnyObject) {
        yearOfBirth.resignFirstResponder();
        // when user do not tap the textfield, the keypad will automaticlly disappear
        
        if let year = yearOfBirth.text.toInt(){
            var imageNumber = (year - offset)%12
            image.image = UIImage(named: String(imageNumber))
            
        }
        else{
            
            //notify the user
        }
    }
        

}

