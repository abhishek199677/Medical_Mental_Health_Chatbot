

conda create -n medical python=3.9 -y  
conda activate medical 
pip install -r requirements.txt
pip freeze #must be done before running the app
uvicorn main:app --host 127.0.0.1 --port 8000 --reload



pip install langchain-openai


lsof -i :8000 