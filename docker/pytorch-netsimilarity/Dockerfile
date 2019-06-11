FROM pytorch/pytorch

RUN apt-get update && apt-get install -y \
    libgtk2.0 \
    fish

RUN conda install -c conda-forge jsmin -y

# Install tqdm for terminal progress bar
RUN conda install -c conda-forge tqdm -y

# Install sklearn
RUN conda install -c anaconda scikit-learn -y

# Cleanup
RUN apt-get clean && \
    apt-get autoremove

CMD fish
