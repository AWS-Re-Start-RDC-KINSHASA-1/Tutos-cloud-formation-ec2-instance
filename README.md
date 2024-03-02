# Tutoriel sur le CloudFormation pour lancer une instance EC2, un groupe cible et un équilibreur de charge

Ce tutoriel vous explique comment lancer une instance, un groupe cible et un équilibreur de charge à partir du CloudFormation. Voici les étapes :

1. Connectez-vous à votre console Amazon.
2. Recherchez "CloudFormation" dans la barre de recherche.
3. Cliquez sur "Créer une nouvelle pile".

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/2f3cf85f-a2ff-4a11-8af6-591227ba43b8)

4. Sélectionnez votre fichier de code au format YAML ou JSON pour créer l'instance et l'équilibreur de charge. Dans mon cas, mon fichier s'appelle "instance.yml" et j'ai utilisé Visual Studio Code pour coder. Vous pouvez trouver mon code sur GitHub si vous souhaitez l'utiliser.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/1f551f46-367d-478e-b083-4cc28d73f9c9)

5. Cliquez sur "Suivant".
6. Nommez votre pile (par exemple, "TestInstance").

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/986fad7e-dfb2-4cea-91be-58ad34a981aa)

7. Cliquez sur "Suivant".
8. Laissez les paramètres par défaut et cliquez sur "Suivant".
9. Cliquez sur "Soumettre" pour créer la pile.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/a325c7c6-4c65-4b8f-9ac2-774e32f3343b)

La création peut prendre un certain temps car chaque bloc de votre code doit être examiné. Actualisez la page pour suivre la progression.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/d1e08a40-6130-4aa6-b888-15b1b3152128)

Après la création, vérifiez dans Amazon EC2 si l'instance et l'équilibreur de charge ont été créés.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/828ba5cd-c862-49e4-bf9d-5eb68ab3c2d1)

Consultez les instances pour voir les instances créées (trois instances) comme indiqué dans l'image.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/d341c522-1a46-4bae-80c0-9e35aaac1520)

Cliquez sur le groupe de mise à l'échelle automatique et l'équilibreur de charge pour vérifier leur création.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/ce24ccf9-e5d6-4cb4-afe6-3b1261ad8137)

Effectuez un test en copiant le nom du DNS de l'équilibreur de charge comme indiqué dans l'image. Cela affichera un "hello world" si vous avez configuré votre site dans le code "instance.yml". Voici le résultat.

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance/assets/114914329/f19b76c4-5c78-470d-944f-47de1db44ea9)

En suivant ces étapes, vous pourrez lancer une instance et un équilibreur de charge à partir du CloudFormation. Assurez-vous de renseigner correctement les ID dans le fichier "instance.yml" en fonction de votre configuration. Vérifiez vos ID de groupe de sécurité, VPC, sous-réseau et paire de clés. Prenez en compte ces modifications pour assurer le bon fonctionnement du processus !

















