PY ?= python3
export PYTHONPATH := src

.PHONY: all data train test demo agent clean

all: data train test

data:          ## simulate, validate and featurise 8,000 production runs
	$(PY) -m offcut.pipeline

train:         ## train P10/P50/P90 models, write metrics, figures and browser model
	$(PY) -m offcut.train

test:
	$(PY) -m unittest discover -s tests -v

demo:          ## forecast -> grade -> match for a sample order (no API key needed)
	$(PY) -m offcut.service

agent:         ## Claude agent on a free-text order note (needs requirements-agent.txt + credentials)
	$(PY) -m offcut.agent "PO 4471: 22k metres white cotton jersey, 180gsm, 1.8m wide, tees S-XXL, shipping from Dhaka"

clean:
	rm -rf data/raw data/staged data/features
