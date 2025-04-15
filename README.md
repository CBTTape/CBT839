# CBT839
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 839 is from Clement Clarke and contains programs to       *   FILE 839
//*           allow for long PARM fields and symbolic parameter     *   FILE 839
//*           substitution in card image format control cards.      *   FILE 839
//*                                                                 *   FILE 839
//*       Description:                                              *   FILE 839
//*                                                                 *   FILE 839
//*          Long Parameters and Symbolic Parameter                 *   FILE 839
//*          replacement in card image control cards.               *   FILE 839
//*                                                                 *   FILE 839
//*       The following programs are now available that will        *   FILE 839
//*       allow the above to happen, using conventional JCL or      *   FILE 839
//*       TSO.                                                      *   FILE 839
//*                                                                 *   FILE 839
//*       1. EXECLONG will execute a program with up to 3,000       *   FILE 839
//*          bytes as a parameter.                                  *   FILE 839
//*                                                                 *   FILE 839
//*       2. PARMCNTL creates either Fixed or Variable blocked      *   FILE 839
//*          control file from a Parameter, or other control        *   FILE 839
//*          file.                                                  *   FILE 839
//*                                                                 *   FILE 839
//*       3. SAVEPARM saves parameters into a VB file which is      *   FILE 839
//*          used by EXECLONG and/or PARMCNTL above.                *   FILE 839
//*                                                                 *   FILE 839
//*       Further Description:                                      *   FILE 839
//*                                                                 *   FILE 839
//*       1. EXECLONG executes the program specified with the       *   FILE 839
//*          PARM='PGM=program-name'.  It first reads a VB file     *   FILE 839
//*          allocated with a DDNAME of $$PARM, and creates a       *   FILE 839
//*          standard parameter of up to 3,000 bytes.               *   FILE 839
//*                                                                 *   FILE 839
//*          Standard APF facilities are used, so Authorised or     *   FILE 839
//*          Non-Authorised programs may be used.                   *   FILE 839
//*                                                                 *   FILE 839
//*       2. PARMCNTL creates either FB or VB control files from    *   FILE 839
//*          either the VB $$PARM file.                             *   FILE 839
//*                                                                 *   FILE 839
//*          PARMCNTL creates a file using the $$CNTL file.  It     *   FILE 839
//*          either takes it's input from the parameter field,      *   FILE 839
//*          or, if that is null, it reads from the $$PARM file.    *   FILE 839
//*                                                                 *   FILE 839
//*          New control cards are created on finding a LF (X'25')  *   FILE 839
//*          character, or <p>.                                     *   FILE 839
//*                                                                 *   FILE 839
//*          After forming up the parameter fields or the records   *   FILE 839
//*          from the $$PARM DD File, the following parameters      *   FILE 839
//*          are allowed:                                           *   FILE 839
//*                                                                 *   FILE 839
//*             PGM=program-name  - Program to be executed.         *   FILE 839
//*             DDN=ddname        - Instead of the $$CNTL,          *   FILE 839
//*                                 use ddsname instead.            *   FILE 839
//*             PARM='parameter'  - Use this parameter.             *   FILE 839
//*                                 Quotes are not allowed.         *   FILE 839
//*                                                                 *   FILE 839
//*       3. SAVEPARM appends it's parameter to the VB $$PARM       *   FILE 839
//*          file.  Symbolic parameters may be used in the PGM      *   FILE 839
//*          PARM field, and hence can be used by the PARMCNTL      *   FILE 839
//*          program to create control files with symbolic          *   FILE 839
//*          parameters replaced.                                   *   FILE 839
//*                                                                 *   FILE 839
//*       This program is provided free of charge, under the        *   FILE 839
//*       Apache Licence, for Hercules and "Hobbyist"               *   FILE 839
//*       licences.                                                 *   FILE 839
//*                                                                 *   FILE 839
//*       However, you are definitely invited to contribute         *   FILE 839
//*       money if you find this software useful. This will         *   FILE 839
//*       assist with the development of new software and           *   FILE 839
//*       similar.                                                  *   FILE 839
//*                                                                 *   FILE 839
//*       There is no warranty - source code is provided so         *   FILE 839
//*       that the program may be maintained.                       *   FILE 839
//*                                                                 *   FILE 839
//*       Note: You may not convert this program into a paid        *   FILE 839
//*             product, and all source code changes must be        *   FILE 839
//*             made available for everyone.                        *   FILE 839
//*                                                                 *   FILE 839
//*       Clement Clarke                                            *   FILE 839
//*                                                                 *   FILE 839
//*       My email is clemclarke@gmail.com                          *   FILE 839
//*                or clementclarke@ozemail.com.au                  *   FILE 839
//*       Tel Australia  Mobile  +61 401 056 155                    *   FILE 839
//*                                                                 *   FILE 839
```
