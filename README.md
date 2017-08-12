# PyNordicRW
Read SEISAN-NORDIC format into a dictionary.

    """
    Input: 'select.out' or any nordic file.
    Output: a dictionary with the following structure:

    out_dic:
           |
           |
            Event_ID_dic:[ex: '20130105123412.7']
                        |
                        |
                        HEADER_dic: [ex: 'L1':{},'LE':{},'LF':{}]
                        |         |
                        |         |
                        |         LINE-1/LINE-E/LINE-F [ex: 'LAT':52.32...]
                        |
                        |
                        PHASE_dic: [ex: 'AAA':{}]
                                 |
                                 | 
                                 P/S_dic: [ex: 'P':{}, 'S':{}]
                                    |
                                    |
                                     INFO: [ex: 'RMS':.03, 'GAP':180.,...]

    """
