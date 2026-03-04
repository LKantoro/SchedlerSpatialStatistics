# A Close look at "A Close look at the structure implied by CAR and SAR models"

## Contributors

-   Julia Schedler, Lucas R. Kantorowski (add yourself once you make a change to the code!)

This repository is focused on replicating and eventually extending the wall 2004 paper.

DOI: [https://doi.org/10.1016/S0378-3758(03)00111-3](https://doi.org/10.1016/S0378-3758(03)00111-3){.uri}

Citation:

Wall, M. M. (2004). A close look at the spatial structure implied by the CAR and SAR models. Journal of Statistical Planning and Inference, 121(2), 311–324.

## Project Structure

-   `ReplicatingWall.qmd` is a work in progress to replicate Table 1 from the paper
    -   `estimates_and_sources.csv` contains parameter estimates (and some standard errors) for the three spatial models and iid model (from Table 1 in the paper)
        -   `data.collection` indicates three possible sources for values:

            -   `transcription` are values manually read from the paper entered in via keyboard

            -   `replication` contains outputs from `ReplicatingWall.qmd`, and should match all values sourced via `transcription`

            -   `generation` is where outputs from models using a different spatial weight matrix will be stored, once the project moves to *Extending* rather than *Replicating.*
-   `wall_2004_dataset.csv` is the data from the original paper, with state names consistent with the `us_states` from `spData`
    -   originally obtained as `state-sat.dat` from the data sets webpage of the wonderful *Hierarchical Modeling and Analysis for Spatial Data, 2nd Edition*, "help yourself" license
