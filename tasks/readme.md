����������� �� ������ � CMake � ������ ������ �����.

������ ����������� ��������� ������� ������ ��� ����� ������� ����� ����������. 

��� ����, ����� ������� ������ � �������� ����� ��������� "���������� �����", ������� �������� ��������� ����:

1. ����� ������ �������, ������� ��������� � solutions\ihar_marozau\< ����� �������� ������ >. 
   ��������, solutions\ihar_marozau\1 ��� 1-�� �������� ������. 

2. ����������� ������ ������� � ���� ������� ���������� /solutions/< user_name >.

3. � ����� sources ���������� ������� ������� ���������� � �������� <�����_������>, ��� "�����_������" - ������������� �������������� ������ � �������, 
   �������� 1_1, 1_2 ��� 1_3 ��� ����� �� 1-�� �������� ������. ��� ����� ��������� � ��������.

4. � ���������� � ����������� ������� ���� CMakeLists.txt �� ��������� �����������: compile_project( ${module_name} "*.cpp" "*.h" BINARY binaries ). 
   ������ ����� ����� �� lections\1\code_examples\cmake_example\sources\functions\
   !!!�����!!! ���������� ����� ����� ����� ���������� �� �������� ������ � �������� ������. �� ����� �������� �������� �� ���������. ������ �����������

5. �������� �������� ����� � ����� � �����������. 

6. ������� CMake ����-��������� ��� ��������������� ����� ����������. �� ������ ����� ����� _msvc_gen_2005_64.bat ��� _gcc_gen.sh. 
   � ������� ������� cmake ���������� �������� ��� ����� ����������. ���������� �� ������ ����� ����� �� ����� cmake.org ��� ���������.
   ��������, ��� Visual Studio 2010 ��������������� ���� _msvc_gen_2005_64.bat � _msvc_gen_2010_64.bat � �������� �������  
   cmake -DVERBOSE=OFF -DCMAKE_BUILD_TYPE=%BUILD_TYPE% -DSOLUTION_NAME=%SOLUTION_NAME%  -G "Visual Studio 8 2005 Win64" ../    
   ��
   cmake -DVERBOSE=OFF -DCMAKE_BUILD_TYPE=%BUILD_TYPE% -DSOLUTION_NAME=%SOLUTION_NAME%  -G "Visual Studio 10 Win64" ../   

7. ��������� ����-��������� �� ��������� ������� Debug ������. ���� �� ������ ������������� Release ������, 
   �� ��� ����� ������� ��������� � ���������� "Release" ( �������� ��� Visual Studio 2005: _msvc_gen_2005_64.bat Release )
   
8. ������ ��� ����� ����� ���������� ����� ����� � ���������� _build_Debug_64 ��� Debug ������� � � _build_Release_64 ��� Release.

9. ������! �������! 

���������������� ����������� ����� ��������� � ����� < ��� cmake ������ >\_build_Debug_64\bin_64\Debug ��� Debug ������� ��������������. 

!!!�����!!! �� ���������� ����� ����� ����������� ���� ����� ����� ����������. ��� ���������� �������� ������ � ������ 
            ����� � ������ ��������� ��� ���������� �� � ����� � �����������, ����� ��������� CMake ���������.
			
!!!�����!!! �� ��������� ��������� ���� ����� � �������� ����� � git (git add). ������ ����� �������� ������. 