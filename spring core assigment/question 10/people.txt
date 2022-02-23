package Question10;

public class People {
	String Name;
	Long Contact;
	
	public People(String name, Long contact) {
		super();
		Name = name;
		Contact = contact;
	}
	public String getName() {
		return Name;
	}
	public void setName(String name) {
		Name = name;
	}
	public Long getContact() {
		return Contact;
	}
	public void setContact(Long contact) {
		Contact = contact;
	}
	
	@Override
	public String toString() {
		return "People [Name=" + Name + ", Contact=" + Contact + "]";
	}
}
