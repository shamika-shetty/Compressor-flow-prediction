
# Compressor flow(cfm) prediction

This business case study project mainly helps the sales engineer to predict what kind of model they can suggest to clients based on cfm flow and other parameters.Generally while buying compressor clients only specify the power and pressure and its hard for the sales engineer to go through all the catalogue and to suggest the compressor model, it is a time consumering process too. So the main aim of this project is to minimize the time of sales engineer to go through catalogue. This project will predict the cfm flow when you input pressure,power and weight.Based on the predicted cfm flow and othe parameters like power, presure,weight it is eay for sales engineer to suggest to clients.


## DataSet
The data for this case study is scrapped from the various catelogues and selected important features that helps in predicting the compressor flow.

* Model : name of the compressor models
* Power : power of a TEFC(Total Enclosed fan cooled motor) moter in KW
* Pressure : pressure of compressed air in bar
* Weight : Weight of the compressor in Kg
* Controller Type : Controller typer based on air end
* flow : The output air flow (cfm). Target variable to be predicted

## Approach
Regressor model is used to predict the flow(cfm).Different models are build out of which XGBoost Regressor gave highest accuracy and the final model is build using the same.
Pipeline is done for the final model and using pickle model is saved.
## Deployment

Deployment is done using Streamlit
( refer : https://docs.streamlit.io/ )

```bash
  streamlit run compressor.py 
```



As a future enhancement for this case study, many data records can be added and few other related features can also be included.