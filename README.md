##  Visuino FUNCTION BLOCK - SEQ (Sequence)

####  written by - me@johnsawyers.com

#### license - Creative Common License CC-BY-NC

#### DESCRIPTION
This function block(FB) provides a method to perform  sequential sequencing. 

####  INPUTS

STEP (BOOL) - A rising signal on this input will advance the block to the next step.
              When STEP5 is active and the STEP input is true, the block will advance to STEP0.

RST (BOOL)  - A rising signal on this input will set the block to STEP0

####  OUTPUTS

STEPx (BOOL) - Indicates that STEPx is active.  Only one STEP output 
               will be active at any one time.

SEQ (UINT) - Indicates active STEP 0 through 5.

####  NOTES:

  (1) The clock input is not needed for this block to function.
