//
//  UITextView.swift
//  WordMate
//
//  Created by AlexK on 13/01/2023.
//

import Foundation
import UIKit

extension UITextView {
    func newHeight(withBaseHeight baseHeight: CGFloat) -> CGFloat {

        // Calculate the required size of the textview
        let fixedWidth = frame.size.width
        let newSize = sizeThatFits(CGSize(width: fixedWidth, height: .greatestFiniteMagnitude))
        var newFrame = frame

        // Height is always >= the base height, so calculate the possible new height
        let height: CGFloat = newSize.height > baseHeight ? newSize.height : baseHeight
        newFrame.size = CGSize(width: max(newSize.width, fixedWidth), height: height)

        return newFrame.height
    }
}
