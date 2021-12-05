# Most-complete-introduction-to-the-use-of-CLAPACK
The name of each function in LAPACK already specifies the rules for using that function.All functions are named in the form XYYZZZ

The first letter X represents the following data types:
S REAL 
D DOUBLE PRECISION
C COMPLEX
Z COMPLEX*16 or DOUBLE COMPLEX

The next two letters YY represent the array type:
BD bidiagonal
DI diagonal
GB general band
GE general (i.e., unsymmetric, in some cases rectangular)
GG general matrices, generalized problem (i.e., a pair of general matrices)
GT general tridiagonal
HB (complex) Hermitian band 
HE (complex) Hermitian
HG upper Hessenberg matrix, generalized problem (i.e a Hessenberg and a triangular matrix)
HP (complex) Hermitian, packed storage
HS upper Hessenberg
OP (real) orthogonal, packed storage
OR (real) orthogonal
PB symmetric or Hermitian positive definite band
PO symmetric or Hermitian positive definite
PP symmetric or Hermitian positive definite, packed storage
PT symmetric or Hermitian positive definite tridiagonal
SB (real) symmetric band 
SP symmetric, packed storage
ST (real) symmetric tridiagonal
SY symmetric
TB triangular band
TG triangular matrices, generalized problem (i.e., a pair of triangular matrices)
TP triangular, packed storage
TR triangular (or in some cases quasi-triangular)
TZ trapezoidal
UN (complex) unitary
UP (complex) unitary, packed storage

The last three letters ZZZ stand for method of calculation
SV solves the general linear equations AX is equal to B
LS computes the least square solution of an overdetermined linear system, A X=B or A**H X=B, or the least norm solution of an indeterminate system
LSE uses GRQ(generalized RQ) decomposition to solve constrained linear least squares problems
GLM solves GLM(generalized linear regression model) using GQR(generalized QR) factorization
EV computes all the eigenvalues and optional eigenvectors of a real symmetric matrix
ES computes the eigenvalues and Schur factorization of a general matrix and sorts the factorization so that the selected eigenvalues are in the upper-left corner of the Schur form
SDD Calculates singular Value Decomposition (SVD) of General Rectangular Matrices by divide-and-conquer
GV computes all eigenvalues and eigenvectors of a generalized symmetric definite generalized eigenproblem (Ax= Bx, ABx= x, or BAx= x)
GS computes the generalized eigenvalues, Schur form, and left and/or right Schur vectors of a pair of matrices
SQR Calculates singular Value Decomposition (SVD) of a Matrix using double diagonal QR algorithm
SNA computes the conditional reciprocal of the eigenvectors of real symmetric or complex Hermitic matrices or the left or right singular vectors of general matrices
BRD reduces the general band matrix to a real bidiagonal form by orthogonal transformation
EQU computes the ratio of rows to columns to balance a general band matrix and reduce its number of conditions
TRF computes the LU factorization of a matrix, using partial rotations with row swaps
TRS solves general linear equations AX=B, A **T X=B or a **H X=B, using SGBTRF computed LU factorization
BAK transforms the eigenvectors of the matrix into eigenvectors of the original matrix supplied to SGEBAL.
CON uses the LU factorization calculated by SGETRF to estimate the reciprocal of the conditional numbers of matrices, whether 1-norm or infinity-norm
HRD reduces a matrix to the upper Hessenberg form by orthogonal similarity transformation
LQF Computes the LQ factorization of a rectangular matrix
QLF computes the QL factorization of a rectangular matrix
QRF computes the QR factorization of a rectangular matrix
TRI computes the inverse of the matrix and uses SGETRF to compute the LU factorization
EIN computes the right and/or left eigenvectors specified by the matrix through inverse iteration
EQR computes the eigenvalues and Schur factor decomposition of a matrix, using the multi-shift QR algorithm
CSD computes the CS decomposition of matrices in the form of double diagonal blocks
RZ Computes the RZ factorization of a matrix
SYL solves the Sylvester matrix equation A X +/ -x B=C
SEN reorders the Schur factorization of the matrix to find the orthonormal basis of the right invariant subspace corresponding to the selected eigenvalues, and returns the reciprocal condition number (sensitivity) of the set of eigenvalues and the mean value of the invariant subspace.
EXC reorders the Schur factorization of matrices by orthogonal similarity transformation
EVC computes some or all of the right and/or left eigenvectors of the matrix
SJA computes the generalized singular value decomposition of the matrix output by SGGSVP
TRD reduces the matrix to a real symmetric tridiagonal form by orthogonal similarity transformation.
