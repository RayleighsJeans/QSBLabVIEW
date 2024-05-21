This is the README for the bolometer QSB LabVIEW VI.

# QSB LabVIEW VI: all branches
    1 - full in-situ calibration and offset (float) voltage measurement
        before experiment with variable fit routine and actual maximum
        current measurement

    2 - modular trigger time setting, either last CODAC on website
        or start time of VI for upload to archive

    3 - either upload to archive & store locally on HDD or do
        only the latter

    4 - DAC range settings either by file ingestion for individual
        settings or global dial for every channel the same

    5 - backup calibration values file input load for lab tests

    6 - skipping first 1000 samples of acquisition because step in signal from
        pin selection

    7 - upload of all the things from the VI created, PARLOG included with
        runtime settings etc
    
    8 - sampling times possible for 0.8, 1.0, 1.6, 3.2, 6.4ms
        assuming maximum sample number ~ 90k-100k

# brach: master & raw_wRTF
    9 - a - use a selection of to estimate/calculate the
            total irradiated power from the plasma in real time
        b - UI interface to input the channels/channel numbers
        c - single channel output alongside using the voltage or power
            multiplied by a single number

    10 - get weighting factors to be used with the channel selection when
         calculating P_rad; get geomtry factors from file.

    11 - a - plot of P_rad estimate from the transmitted samples
         b - add the "true" P_rad after the shot to this plot from both cameras
         c - writes the full P_rad and the estimate plus single channel
             feedback to the archive.

    12 - double channel voltage output via the references handed over to the
         hReadChannelsUandP for single values of channel and P_rad;
         also possible to skip feedback inside DAQ, button on front panel
