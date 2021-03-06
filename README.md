# Toolkit instructions

The toolkit is useful for getting the corresponding label map for [the PASCAL Part Challenge](http://www.stat.ucla.edu/~xiaochen.lian/paspart_challenge/index.html)

For the toolkit, it includes the code translate [PASCAL part data](http://www.stat.ucla.edu/~xianjie.chen/pascal_part_dataset/pascal_part.html) into the evaluation semantic part labels. 


For translate the labels: 

 	Download the pascal part from the website and unzip it to trainval folder 
 	(the annotation should be under $PATH/trainval/Annotations_Part). 
 	
	Run $PATH/Toolkit/demo.m to check the examples of mapping the part label annotations to the evaluation part (also the instance bounding boxes). 

	We also included the object localization method used in our paper if you want to use exactly the same localization for comparison (Check localizeObj_v2.m).

For the labels' semantic meaning of the transfered part id map. 

	Run $PATH/Toolkit/LoadPascalPart.m
        The meanning of generated struct is listed as follows: 

	VOCPart.SemPartNames: mapid to semantic part names 
	VOCPart.obj_id: the correspondent semantic class id to the VOC objects. 
	VOCPart.classes: the semantic class name 
	VOCPart.classes_all: original VOC objects names. 

This toolkit is provided and used to generate the ground truth used in the following paper: 
	
	@article{wang2015joint,
	  title={Joint Object and Part Segmentation using Deep Learned Potentials},
	  author={Wang, Peng and Shen, Xiaohui and Lin, Zhe and Cohen, Scott and Price, Brian and Yuille, Alan},
	  journal={ICCV},
	  year={2015}
	}

Any problems,  contact pengwangpku2012@gmail.com 

We will later try to release our model and code, but it might depend on the authors' time. 
