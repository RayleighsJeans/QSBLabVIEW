Here comes the setup for equivalently working data acquisition PCs.

$ ########################################################################## $

  1 -- Install your hardware. Used in this specific case is:
       (W7-X, setup anno ~2015) we used:
        A -- NI PCI 7813R (NI RIO FPGA Device) with an ADC 7730
        B -- NI PCIe 6321(R) [connected to --> C -- BNC 2090A]
       (D -- potentially a NI PCI 7638(R)/7681(R))

  2 -- Install the specific hardware drivers. Either get them directly
       from the provided CD/USB by the manufacturer (National Instruments)
       OR: They can be found in the UNTOUCHED setup directory located in the
       W7-X physics network in:

            \\sv-di-fs-1\E5\E5-IMP\Bolometer\Software\ ...
                ... \LabvView_Setup\Installation_Library\  .

      Choose the 32bit version. Especially make sure you
      have all drivers and libraries installed that are required to access
      your hardware properly. (LIC=M63X86661)

  3 -- Also install the DAQ framework and the National Instruments 'NIMax'
       device / software interface which includes LabVIEW.

  4 -- You are done (sort of ...).
       Test by trying to compile the initially commited
       VI from March 2018 (dd8e1c887985f614fc7a74ad8111f8b08ac6b97b).

       To do so: Load up the *.lvproj file (whatever it is called on
       the wildcard). At the very bottom of the dependency tree select
       Build Preferences/Build Specifications
       Then select the dropped box. Here, customize whatever you want
       (preferably *.exe for me) and click on build in the bottom button bar.
       If successful, setup is successful.

For further questions, please do not hesitate to ask via:
   pih@ipp.mpg.de  <--- primary contact
  (flr@ipp.mpg.de)
  (daz@ipp.mpg.de)

$ ########################################################################## $