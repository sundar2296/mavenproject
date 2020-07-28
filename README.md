# mavenproject
excel files

public class excelread {

	public static void main(String[] args) throws IOException {
		File f=new File("D:\\selenium\\mavenproject.org\\Excel\\selenium.xlsx");
		FileInputStream Stream= new FileInputStream(f);
		Workbook w = new XSSFWorkbook(Stream);
		Sheet s=w.getSheet("Data");
		//row
		Row r =s.getRow(0);
		Cell c =r.getCell(0);
		System.out.println(c);
		
		
	}

}
