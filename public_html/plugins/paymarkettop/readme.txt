ReadME.md
# starlance-theme-ua
### ��������� ���������� �� ���� ���� ������������ ������ ������ �� ������
# UA Freelance Marketplace
## ��������� ������ ��������� �������, ��������� �� ������� ������ �����������. 
## ������ ������ ����� ������������ �� ������ ������ 2022 ���� �� PHP v. 7.4
# 


===
## �������
	https://github.com/webitproff/
===
## ������������ �� ����� ��������� ��� ������ ������������ �� CMF Cotonti
	http://freelance-script.abuyfile.com/
	https://www.facebook.com/CMS.Freelance
	https://t.me/s/cotonti
===
## �i�����������
	https://www.youtube.com/playlist?list=PLLJqscgzN-F4PmZnbYDsXUYfbT4rxC9Dz
===
## ��������-������� ������� ����� (������ ��������� ���)
	https://abuyfile.com/
===
## �������� ��� ����������� ��������:
	� Email: webitproff@gmail.com
	� Telegram: https://t.me/webitproff
===
��������� ���� ��������� ���������� ��� ��� ������� �� ����������, �� ���������� 

# 
===


������ ��������� ������������ ������� ������ �� �������� ������ � ������.

��������������� ����������� ��������:

    ���������� ��������� � ����� plugins ������ �����.
    ������� � ������ �������������� � ���������� ������ ������.
    � ���������� ������� ������� ��������� ������ �� ���� ����.
    ����� ���������� �������� ��� ��� ������ �� ������ ������ � ������� market.userdetails.tpl ����:

    	
    <!-- IF {PHP.cot_plugins_active.paymarkettop} AND {PHP.usr.id} == {PHP.urr.user_id} -->
           {PRD_ROW_PAYTOP}
    <!-- ENDIF -->

    ��� � ����� ������ ������� market.list.tpl:

    <!-- IF {PHP.cot_plugins_active.paymarkettop} AND {PHP.usr.id} == {PRD_ROW_OWNER_ID} -->
           {PRD_ROW_PAYTOP}
    <!-- ENDIF -->

    ��� ����������� ������� �� �������� ������ � ������� market.tpl:

    	
    <!-- IF {PHP.cot_plugins_active.paymarkettop} AND {PHP.usr.id} == {PRD_OWNER_ID} -->
           {PRD_PAYTOP}
    <!-- ENDIF -->

    ������ �� ������ ������ ����� ������������ ������ ��������� ������.

    ����� � ����� ������ ������� ���������� ��������� ����� ��� ���-�������, ��� ������� ������������ ������.
    ��� ����� � ������� market.list.tpl ������ ����� <!-- BEGIN: PRD_ROWS --> � �����, ������� ��������� ����� � ������, ���������� ��������� ������� ��� ���������� �����, ��������:

    	
    <div class="media<!-- IF {PRD_ROW_ISTOP} --> prdtop<!-- ENDIF -->">

    ����� ����� � css ����� ����� ���� �� �������� ��������� ����� ��� ���-������ .prdtop, �������� ���:

    	
    .prdtop { background-color: #feefb3; }