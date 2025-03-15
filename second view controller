import UIKit

class SecondViewController: UIViewController{
    @IBAction func pristupim(_ sender: Any) {
    }
    @IBOutlet weak var cloud: UIImageView!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        
        
        let imageView = UIImageView(image:UIImage(named: "frogsecond"))
        imageView.frame = CGRect(x:10, y:400, width: 300, height: 270)
        imageView.contentMode = .scaleAspectFit
        view.addSubview(imageView)
        
        let cloud = UIImageView(image:UIImage(named: "cloude"))
        cloud.frame = CGRect(x:90, y:50, width: 300, height: 400)
        cloud.contentMode = .scaleAspectFit
        view.addSubview(cloud)
        
       
        let pristupim = UIButton(type: .custom)
        pristupim.setImage(UIImage(named: "pristupim"), for: .normal)
        // Укажи позицию и размер кнопки
        pristupim.frame = CGRect(x: 75, y: 720, width: 260, height: 58)
        view.addSubview(pristupim)
     
        pristupim.addTarget(self, action: #selector(pristupimTapped), for: .touchUpInside)
    }
    
            @objc func pristupimTapped() {
            let storyboard = UIStoryboard(name: "Main", bundle: nil)
            if let thirdVC = storyboard.instantiateViewController(withIdentifier: "ThirdViewController") as? ThirdViewController {
                thirdVC.modalPresentationStyle = .fullScreen // Полноэкранный режим
                present(thirdVC, animated: true, completion: nil)
            }
        }
        
    }
