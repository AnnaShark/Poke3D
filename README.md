# Poke3D

An app that adds 3d models of pokemons to pokemon cards. Now has only Pikachu and Charmander. 

To add more cards and models you need to: 

1. Make a photo of a pokemon card and drag it to Assets.xcassets/Pokemon cards. Name the card with the name of a pokemon you want to add. If you do not have cards, you can print any from this site > https://limitlesstcg.com/tools/proxies/
2. Go to this site and donwload a 3D model for that pokemon > https://free3d.com/3d-models/oddish
3. Drag the downloaded model directory to art.scnassets directory in the project.
4. Chose file with .DAE extension, choose Editor in the upper menu of Xcode and choose convert to scn file.
5. In the ViewController.swift file in renderer method add another ```if imageAnchor.referenceImage.name == " put yuur pokemon card name here"```, and inside the if statememnt change the link to your .scn file in line  ```if let pokeScene = SCNScene(named: "art.scnassets/Pikachu/YourScnFileHere.scn")```
6. Probably in the 3D model you will need to adjust the scale to a smaller one, as usually they are big. You can do it by clicking on the model in preview and changing configs in the right panel.




![](poke3D.gif)
