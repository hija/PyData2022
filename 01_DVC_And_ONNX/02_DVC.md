# DVC

I ran the following commands to test DVC, after I created two models in the data directory:


    dvc init
    git commit -m "Added DVC" 
    
    dvc add 01_DVC_And_ONNX/data/wine_dt_cf.onnx
    dvc add 01_DVC_And_ONNX/data/wine_dt_cf_vuln.bin

    git add 01_DVC_And_ONNX/data/.gitignore 01_DVC_And_ONNX/data/wine_dt_cf.onnx.dvc 01_DVC_And_ONNX/data/wine_dt_cf_vuln.bin.dvc
    git commit -m "Added raw DVC data"

    dvc remote add -d storage /tmp/testdvc
    dvc push
    
    git add .dvc/config
    git commit -m "Configure remote storage"


Then I deleted the two models (.onnx and .bin file) from the direct data directory and ran `dvc pull` and the model was retrieved correctly :-)


    